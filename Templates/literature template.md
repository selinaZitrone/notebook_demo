---
year: {{date | format("YYYY")}}
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
created: {{date | format("YYYY-MM-DD HH:MM")}}
tags: 
---
# title:: {{title}}

authors:: {{authors}}
{% for t in tags %}#paper/{{t.tag}}{% if not loop.last %}, {% endif %}{% endfor %}

[Open Zotero Entry](zotero://open-pdf/library/items/{{itemKey}})

{%- for attachment in attachments | filterby("path", "endswith", ".pdf") %}[Read PDF in Zotero](zotero://open-pdf/library/items/{{attachment.itemKey}}){%- endfor %}

> [!Cite] Citation  
> {{bibliography}}  

> [!Abstract]  
> {%- if abstractNote %}  
> {{abstractNote}}
> {%- endif -%}
> 

# My notes
  
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