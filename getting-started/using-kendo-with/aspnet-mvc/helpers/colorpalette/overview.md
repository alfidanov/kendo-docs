---
title: Overview
meta_title: How to use ColorPalette HtmlHelper extension | Kendo UI documentation
meta_description: User Guide for server-side wrapper for Kendo UI ColorPalette for ASP.NET MVC widget.
slug: mvc-colorpalette-overview
publish: true
---

# ColorPalette

The ColorPalette HtmlHelper extension is a server-side wrapper for the [Kendo UI ColorPalette](/kendo-ui/api/web/colorpalette) widget.

## Getting Started

Here is how to configure a simple Kendo ColorPalette:

1.  Make sure you have followed all the steps from the [Introduction](/kendo-ui/getting-started/using-kendo-with/aspnet-mvc/introduction) help topic.

2.  Create a new action method which renders the view:

        public ActionResult Index()
        {
            return View();
        }
3.  Add a color palette:
    - WebForms

            <%: Html.Kendo().ColorPalette()
                    .Name("colorpalette") // The name of the colorpalette is mandatory. It specifies the "id" attribute of the widget.
                    .Value("#ff0000") // Set the value of the colorpalette
            %>
    - Razor

            @(Html.Kendo().ColorPalette()
                  .Name("colorpalette") //The name of the colorpalette is mandatory. It specifies the "id" attribute of the widget.
                  .Value("#ff0000") //Set the value of the colorpalette
            )

## Accessing an Existing ColorPalette

You can reference an existing ColorPalette instance via [jQuery.data()](http://api.jquery.com/jQuery.data/).
Once a reference has been established, you can use the [API](/kendo-ui/api/web/colorpalette#methods) to control its behavior.


### Accessing an existing ColorPalette instance

    //Put this after your Kendo ColorPalette for ASP.NET MVC declaration
    <script>
    $(function() {
        // Notice that the Name() of the colorpalette is used to get its client-side instance
        var colorpalette = $("#colorpalette").data("kendoColorPalette");
    });
    </script>


## Handling Kendo UI ColorPalette events

You can subscribe to all [events](/kendo-ui/api/web/colorpalette#events) exposed by Kendo UI ColorPalette:

### WebForms - subscribe by handler name

    <%: Html.Kendo().ColorPalette()
            .Name("colorpalette")
            .Events(e => e
                .Change("colorpalette_change")
            )
    %>
    <script>
        function colorpalette_change() {
            // Handle the change event
        }
    </script>


### Razor - subscribe by handler name

    @(Html.Kendo().ColorPalette()
          .Name("colorpalette")
          .Events(e => e
                .Change("colorpalette_change")
          )
    )
    <script>
        function colorpalette_change() {
            // Handle the change event
        }
    </script>


### Razor - subscribe by template delegate

    @(Html.Kendo().ColorPalette()
          .Name("colorpalette")
          .Events(e => e
              .Change(@<text>
                function() {
                    // Handle the change event inline
                }
                </text>)
          )
    )

