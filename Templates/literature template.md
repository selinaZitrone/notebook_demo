---
title: "{{title | escape}}"
authors: {{authors}}
year: {{date | format("YYYY")}}
type: {{itemType}}
citekey: {{citekey}}
journal: {{publicationTitle}}
volume: {{volume}}
issue: {{issue}} 
book: {{publicationTitle}}
publisher: {{publisher}}
location: {{place}}
pages: {{pages}}
DOI: {{DOI}}
ISBN: {{ISBN}}
date added: {{exportDate | format("DD/MM/YYYY")}}
---
# {{title}}
{{authors}}

{% if hashTags %}{{hashTags}}{% endif %}

[Open Zotero Entry](zotero://open-pdf/library/items/{{itemKey}})

{%- for attachment in attachments | filterby("path", "endswith", ".pdf") %}[Read PDF in Zotero](zotero://open-pdf/library/items/{{attachment.itemKey}}){%- endfor %}

> [!Cite] Citation  
> {{bibliography}}  

> [!Abstract]-
> {%- if abstractNote %}  
> {{abstractNote}}
> {%- endif -%}
> 
# Reading notes
{% persist "notes" %}
{% endpersist %}
# Annotations
{% persist "annotations" %}
{% set annots = annotations | filterby("date", "dateafter", lastImportDate) -%}
{% if annots.length > 0 %}

#### Imported on {{importDate | format("YYYY-MM-DD h:mm a")}}

{% for annot in annots -%}{%- if annot.annotatedText %}

>[!quote] Quote
{{annot.annotatedText}} [(p. {{annot.pageLabel}})](zotero://open-pdf/library/items/{{annot.attachment.itemKey}}?page={{annot.pageLabel}}&annotation={{annot.id}})

{%- endif -%}

{%- if annot.imageRelativePath %}

>[!quote] Image
![[{{annot.imageRelativePath}}]]

{%- endif %}

{%- if annot.comment %}

>[!annot] Comment
>{{annot.comment}}
 {%- endif %}

{%- endfor %}
{%- endif %}
{%- endpersist %}