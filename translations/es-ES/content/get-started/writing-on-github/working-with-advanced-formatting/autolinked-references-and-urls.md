---
title: Referencias y direcciones URL autovinculadas
intro: 'Las referencias a las direcciones URL, propuestas, solicitudes de extracción y confirmaciones se acortan automáticamente y se convierten en vínculos.'
redirect_from:
  - /articles/autolinked-references-and-urls
  - /github/writing-on-github/autolinked-references-and-urls
  - /github/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
shortTitle: Referencias auto-enlazadas
---

## Direcciones URL

{% data variables.product.product_name %} automáticamente crea vínculos desde las direcciones URL estándar.

`Visita https://github.com`

![URL autovinculada presentada](/assets/images/help/writing/url-autolink-rendered.png)

Para obtener información sobre cómo crear vínculos, consulta "[Sintaxis de escritura y formato básicos](/articles/basic-writing-and-formatting-syntax/#links)".

## Propuestas y solicitudes de extracción

Dentro de las conversaciones en {% data variables.product.product_name %}, las referencias a las propuestas y solicitudes de extracción se convierten automáticamente en vínculos acortados.

{% note %}

**Nota:** Las referencias autovinculadas no se crearon en páginas wikis o archivos en un repositorio.

{% endnote %}

| Tipo de referencia                                                                      | Referencia en bruto                            | Vínculo acortado                                                       |
| --------------------------------------------------------------------------------------- | ---------------------------------------------- | ---------------------------------------------------------------------- |
| URL de propuesta o solicitud de extracción                                              | https://github.com/jlord/sheetsee.js/issues/26 | [#26](https://github.com/jlord/sheetsee.js/issues/26)                  |
| `#` y número de propuesta o de solicitud de cambios                                     | #26                                            | [#26](https://github.com/jlord/sheetsee.js/issues/26)                  |
| `GH` y número de propuesta y solicitud de extracción                                    | GH-26                                          | [GH-26](https://github.com/jlord/sheetsee.js/issues/26)                |
| `Nombre de usuario/N.º de repositorio` y número de propuesta o solicitud de extracción. | jlord/sheetsee.js#26                           | [jlord/sheetsee.js#26](https://github.com/jlord/sheetsee.js/issues/26) |
| `Organization_name/Repository#` y número propuesta o solicitud de extracción            | github/linguist#4039                           | [github/linguist#4039](https://github.com/github/linguist/pull/4039)   |

{% ifversion fpt or ghec %}
Si referencias una propuesta, solicitud de cambios o debate en una lista, la referencia se desplegará para mostrar el título y el estado en su lugar. Para obtener más información acerca de las listas de tareas, consulta la sección "[Acerca de las listas de tareas](/issues/tracking-your-work-with-issues/creating-issues/about-task-lists)".
{% endif %}

## Etiquetas
When referencing the URL of a label in Markdown, the label is automatically rendered. Only labels of the same repository are rendered, URLs pointing to a label from a different repository are rendered as any [URL](/get-started/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls#urls).

The URL of a label can be found by navigating to the labels page and clicking on a label. For example, the URL of the label "enhancement" in our public [docs repository](https://github.com/github/docs/) is

```md
https://github.com/github/docs/labels/enhancement
```

## Confirmar SHA

Las referencias a un hash SHA de confirmación se convertirán automáticamente en enlaces acortados para la confirmación en {% data variables.product.product_name %}.

| Tipo de referencia        | Referencia en bruto                                                                                                                                                            | Vínculo acortado                                                                                                    |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------- |
| URL de confirmación       | [`https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e`](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e) | [a5c3785](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e)                     |
| SHA                       | a5c3785ed8d6a35868bc169f07e40e889087fd2e                                                                                                                                       | [a5c3785](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e)                     |
| User@SHA                  | jlord@a5c3785ed8d6a35868bc169f07e40e889087fd2e                                                                                                                                 | [jlord@a5c3785](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e)               |
| `Username/Repository@SHA` | `jlord/sheetsee.js@a5c3785ed8d6a35868bc169f07e40e889087fd2e`                                                                                                                   | [`jlord/sheetsee.js@a5c3785`](https://github.com/jlord/sheetsee.js/commit/a5c3785ed8d6a35868bc169f07e40e889087fd2e) |

## Personalizar enlaces automáticos a recursos externos

{% data reusables.repositories.autolink-references %}

## Leer más

- "[Sintaxis de escritura y formato básicos](/articles/basic-writing-and-formatting-syntax)"
