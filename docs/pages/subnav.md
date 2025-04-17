# Subnav

<p class="uk-text-lead">Defines different styles for a sub navigation.</p>

## Usage

To apply this component, use the following classes. To align a subnav, for example to horizontally center it, you can use the [Flex component](flex.md).

| Class         | Description                                                                                                         |
|---------------|---------------------------------------------------------------------------------------------------------------------|
| `.uk-subnav`  | Add this class to a `<ul>` element to define the Subnav component. Use `<a>` elements as nav items within the list. |
| `.uk-active ` | Add this class to a list item to apply an active state.                                                             |
| `.uk-disabled`   | Add this class to a list item to apply a disabled state and use a `<span>` instead of an `<a>` element.                        |

```html
<ul class="uk-subnav">
    <li class="uk-active"><a href=""></a></li>
    <li><a href=""></a></li>
    <li class="uk-disable"><span></span></li>
</ul>
```

```example
<ul class="uk-subnav" uk-margin>
    <li class="uk-active"><a href="#">Active</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
    <li class="uk-disable"><span>Disabled</span></li>
</ul>
```

**Note** For a better layout, if items should wrap into the next row, add the `uk-margin` attribute from the [Margin component](margin.md).

***

## Divider modifier

Add the `.uk-subnav-divider` class to separate menu items with lines.

```html
<ul class="uk-subnav uk-subnav-divider">…</ul>
```

```example
<ul class="uk-subnav uk-subnav-divider" uk-margin>
    <li class="uk-active"><a href="#">Active</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>
```

***

## Pill modifier

Add the `.uk-subnav-pill` class to highlight the active menu item with a background.

```html
<ul class="uk-subnav uk-subnav-pill">…</ul>
```

```example
<ul class="uk-subnav uk-subnav-pill" uk-margin>
    <li class="uk-active"><a href="#">Active</a></li>
    <li><a href="#">Item</a></li>
    <li><a href="#">Item</a></li>
</ul>
```

***

## Subnav and Dropdown

You can also use a dropdown from the [Dropdown component](dropdown.md) with a subnav.

```html
<ul class="uk-subnav">
    <li>

        <!-- This is the menu item toggling the dropdown -->
        <a href=""></a>

        <!-- This is the dropdown -->
        <div uk-dropdown="mode: click">
            <ul class="uk-nav uk-dropdown-nav">…</ul>
        </div>

    </li>
</ul>
```

```example
<ul class="uk-subnav uk-subnav-pill" uk-margin>
    <li class="uk-active"><a href="#">Active</a></li>
    <li><a href="#">Item</a></li>
    <li>
        <a href>More <span uk-icon="icon: triangle-down"></span></a>
        <div uk-dropdown="mode: click">
            <ul class="uk-nav uk-dropdown-nav">
                <li class="uk-active"><a href="#">Active</a></li>
                <li><a href="#">Item</a></li>
                <li class="uk-nav-header">Header</li>
                <li><a href="#">Item</a></li>
                <li><a href="#">Item</a></li>
                <li class="uk-nav-divider"></li>
                <li><a href="#">Item</a></li>
            </ul>
        </div>
    </li>
</ul>
```
