---
title: Overview
page_title: Overview
description: "Learn the basics when working with the Telerik UI ExpansionPanel HtmlHelper for {{ site.framework }}."
previous_url: /helpers/navigation/expansionpanel/overview
slug: htmlhelpers_expansionpanel_aspnetcore
position: 1
---

# ExpansionPanel HtmlHelper Overview

The Telerik UI ExpansionPanel HtmlHelper for {{ site.framework }} is a layout component that provides the user with an easy way to expand and collapse a content area within the application.

The Telerik UI ExpansionPanel HtmlHelper is a server-side wrapper for the [Kendo UI ExpansionPanel](/api/javascript/ui/expansionpanel) widget.


* [Demo page for the Drawer](https://demos.telerik.com/{{ site.platform }}/expansionpanel/index)

## Initializing the ExpansionPanel

The following example demonstrates how to define the ExpansionPanel by using the ExpansionPanel HtmlHelper.

```Razor
    @(Html.Kendo().ExpansionPanel()
            .Name("brazil")
            .Title("Brazil")
            .SubTitle("South America")
            .Expanded(true)
            .Content("The word 'Brazil' likely comes from the Portuguese word for brazilwood, a tree that once grew plentifully along the Brazilian coast. In Portuguese, brazilwood is called pau-brasil, with the word brasil commonly given the etymology 'red like an ember', formed from brasa ('ember') and the suffix -il (from -iculum or -ilium). As brazilwood produces a deep red dye, it was highly valued by the European textile industry and was the earliest commercially exploited product from Brazil.")
            )
```

## Referencing Existing Instances

The following example demonstrates how to get an instance of the ExpansionPanel.

```Razor
    @(Html.Kendo().ExpansionPanel()
            .Name("brazil")
            .Title("Brazil")
            .SubTitle("South America")
            .Expanded(true)
            .Content("...")
            )

    <script type="text/javascript">
        $(function () {
            // The Name() of the Drawer is used to get its client-side instance.
            var expansionPanel = $("#brazil").data("kendoExpansionPanel");
            console.log(expansionPanel);
        });
    </script>
```

## See Also

* [Basic Usage of the Drawer HtmlHelper for {{ site.framework }} (Demo)](https://demos.telerik.com/{{ site.platform }}/expansionpanel)
* [Using the API of the Drawer HtmlHelper for {{ site.framework }} (Demo)](https://demos.telerik.com/{{ site.platform }}/expansionpanel/api)
* [Server-Side API](/api/expansionpanel)
