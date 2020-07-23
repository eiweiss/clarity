---
title: Overview
toc: true
---

Button groups are for creating collections of similar type action buttons.

## Usage

Button groups follow normal Button design guidelines. All Button options regarding classes and sizes apply to Button Groups. All features below are available with Solid, Outline and Flat in normal and small sizes.

Button groups can be also used as alternatives for checkboxes and radio buttons.

### Button Groups as Checkboxes

Use when a small list of options can be selected from, similar to the Checkbox component

- blue indicates an option is selected, white (outline) indicates an unselected option
- user can click the button to select, and click again to deselect
- can be configured with preselected options

::: do Use option labels that are 1-3 short words.

<div class="btn-group">
  <div class="checkbox btn">
    <input type="checkbox" id="btn-demo-check-1">
    <label for="btn-demo-check-1">Apples</label>
  </div>
  <div class="checkbox btn">
    <input type="checkbox" id="btn-demo-check-2" checked>
    <label for="btn-demo-check-2">Oranges</label>
  </div>
  <div class="checkbox btn">
    <input type="checkbox" id="btn-demo-check-3">
    <label for="btn-demo-check-3">Kiwis</label>
  </div>
  <div class="checkbox btn">
    <input type="checkbox" id="btn-demo-check-4" checked>
    <label for="btn-demo-check-4">Pears</label>
  </div>
</div>
:::

::: dont Use option labels that are long or more than 3 words.

<div class="btn-group">
  <div class="checkbox btn">
    <input type="checkbox" id="cb-4" checked class="btn" />
    <label for="cb-4">Apples</label>
  </div>
  <div class="checkbox btn">
    <input type="checkbox" id="cb-5" class="btn" />
    <label for="cb-5">Fresh Local Gold Kiwis</label>
  </div>
</div>
:::

### Button Groups as Radio Buttons

Use when selecting one option from a small list of options, similar to the Radio component

- blue indicates an option is selected, white (outline) indicates an unselected option
- user can click the button to select, and click again to deselect
- can be configured with preselected options

::: do Use option labels that are 1-3 short words.

<div class="btn-group">
  <div class="radio btn">
    <input type="radio" name="btn-group-radios" id="btn-radio-1" checked>
    <label for="btn-radio-1">Pears</label>
  </div>
  <div class="radio btn">
    <input type="radio" name="btn-group-radios" id="btn-radio-2">
    <label for="btn-radio-2">Kiwis</label>
  </div>
  <div class="radio btn">
    <input type="radio" name="btn-group-radios" id="btn-radio-3">
    <label for="btn-radio-3">Oranges</label>
  </div>
</div>
:::

::: dont Use option labels that are long or more than 3 words.

<div class="btn-group">
  <div class="radio btn">
    <input type="radio" name="btn-group-radios-1" id="btn-radio-4" checked>
    <label for="btn-radio-4">Pears</label>
  </div>
  <div class="radio btn">
    <input type="radio" name="btn-group-radios-1" id="btn-radio-5">
    <label for="btn-radio-5">Fresh Local Gold Kiwis</label>
  </div>
</div>
:::

## Types

<clr-row>

::: col Solid button groups direct the user's attention to the _primary actions_ the application is suggesting the user take.

<div class="btn-group btn-primary">
  <button class="btn">Solid</button>
  <button class="btn">Group</button>
</div>
:::

::: col Outline groups are used to indicate a set of _secondary actions_ or to reduce the visual noise on a page.

<div class="btn-group">
  <button class="btn">Outline</button>
  <button class="btn">Group</button>
</div>
:::

::: col Flat button groups are used as a set of _tertiary actions_. They are also typically used in Cards and above Datagrids.

<div class="btn-group btn-link">
  <button class="btn">Flat</button>
  <button class="btn">Group</button>
</div>
:::

</clr-row>

### Mixed Classes

#### Button Arrangement

::: do Arrange primary actions on the left, followed by secondary actions, and warning actions as the last button in a group.

<div class="btn-group btn-primary">
  <button class="btn">Favorite</button>
  <button class="btn btn-success">Add</button>
  <button class="btn btn-danger">Delete</button>
</div>
:::

::: dont Arrange warning actions as the first button in a group or have secondary actions before primary actions.

<div class="btn-group btn-primary">
  <button class="btn btn-danger">Delete</button>
  <button class="btn btn-success">Add</button>
  <button class="btn">Favorite</button>
</div>
:::

#### Group Style

::: do Mix similar styled classes together to suit the solution's needs.

<div class="btn-group btn-primary">
  <button class="btn">Create</button>
  <button class="btn">Favorite</button>
  <button class="btn" disabled>Download</button>
</div>
:::

::: dont Mix differently styled classes together, like solid and outlined.

<div class="btn-group btn-primary">
  <button class="btn">Create</button>
  <button class="btn">Favorite</button>
  <button class="btn btn-outline-success" disabled>Download</button>
</div>
:::

## Antomy

There are sevel layout options for button groups, including icon button groups, and button groups with overflow.

### Icon Button Groups

#### Types & Sizes

::: do Icon button groups are available in the solid, outline, and flat types. It’s also best to use the normal (36px) sized ones. This makes them easier to recognize and to click.

<div class="btn-group btn-primary btn-icon">
  <button class="btn">
    <cds-icon inverse shape="check" title="check"></cds-icon>
  </button>
  <button class="btn">
    <cds-icon inverse shape="home" title="home"></cds-icon>
  </button>
  <button class="btn">
    <cds-icon inverse shape="user" title="user"></cds-icon>
  </button>
</div>
:::

::: dont Use small icon buttons in most cases. They are difficult to see and distinguish what the icon is or represents. They also create smaller click targets, making them harder to click.

<div class="btn-group btn-primary btn-sm btn-icon">
  <button class="btn">
    <cds-icon inverse shape="check" title="check"></cds-icon>
  </button>
  <button class="btn">
    <cds-icon inverse shape="home" title="home"></cds-icon>
  </button>
  <button class="btn">
    <cds-icon inverse shape="user" title="user"></cds-icon>
  </button>
</div>
:::

#### With Text

::: do If you have the space, adding text helps users understand the action. Start icon buttons with icons and follow with text.

<div class="btn-group btn-primary">
  <button class="btn">
    <cds-icon inverse shape="check"></cds-icon> Check
  </button>
  <button class="btn">
    <cds-icon inverse shape="home"></cds-icon> Home
  </button>
  <button class="btn">
    <cds-icon inverse shape="user"></cds-icon> User Profile
  </button>
</div>
:::

::: dont Start icon buttons with text and follow with icon. This makes them more difficult to scan quickly.

<div class="btn-group btn-primary">
  <button class="btn">
    Check <cds-icon inverse shape="check"></cds-icon>
  </button>
  <button class="btn">
    Home <cds-icon inverse shape="home"></cds-icon>
  </button>
  <button class="btn">
    User Profile <cds-icon inverse shape="user"></cds-icon>
  </button>
</div>
:::

### Button Groups with Overflow

Overflow is used when the button group is larger than its containing space, or used to preserve space. The overflow is configurable so you can assign button actions to the dropdown menu.

- Overflow button is shown below as an ellipsis button in the button group and is the last position to the right
- Clicking on the ellipsis will show the overflow dropdown menu

::: do Use the overflow as the last item in the button group.

<div class="btn-group btn-primary">
  <button class="btn">Create</button>
  <button class="btn">Favorite</button>
  <div class="btn-group-overflow open">
    <button class="btn dropdown-toggle">
      <cds-icon inverse shape="ellipsis-horizontal" title="Expand dropdown"></cds-icon>
    </button>
    <div class="dropdown-menu">
      <button class="btn">Download</button>
      <button class="btn">Delete</button>
    </div>
  </div>
</div>
:::

::: dont Never place the overflow at the beginning or middle of a button group.

<div class="btn-group btn-primary">
  <div class="btn-group-overflow open">
    <button class="btn dropdown-toggle">
      <cds-icon inverse shape="ellipsis-horizontal" title="Expand dropdown"></cds-icon>
    </button>
    <div class="dropdown-menu">
      <button class="btn">Download</button>
      <button class="btn">Delete</button>
    </div>
  </div>
  <button class="btn">Create</button>
  <button class="btn">Favorite</button>
</div>
:::

#### Icons

Button groups with text and icons, or just icons, will have text show in the dropdown menu
Text for each action icon is needed for overflow to work properly

<clr-row>

::: col

<div class="btn-group btn-primary">
  <button class="btn">Create</button>
  <button class="btn">Favorite</button>
  <div class="btn-group-overflow open">
    <button class="btn dropdown-toggle">
      <cds-icon inverse shape="ellipsis-horizontal" title="Expand dropdown"></cds-icon>
    </button>
    <div class="dropdown-menu">
      <button class="btn">Download</button>
      <button class="btn">Delete</button>
    </div>
  </div>
</div>
:::

::: col

<div class="btn-group btn-primary btn-icon">
  <button class="btn">
    <cds-icon inverse shape="check" title="Add"></cds-icon>
  </button>
  <button class="btn">
    <cds-icon inverse shape="folder" title="Folder"></cds-icon>
  </button>
  <div class="btn-group-overflow open">
    <button class="btn dropdown-toggle">
      <cds-icon inverse shape="ellipsis-horizontal" title="Expand dropdown"></cds-icon>
    </button>
    <div class="dropdown-menu">
      <button class="btn">
        <cds-icon inverse shape="download"></cds-icon>
        <span class="cds-icon-title">Download</span>
      </button>
      <button class="btn">
        <cds-icon inverse shape="refresh"></cds-icon>
        <span class="cds-icon-title">Refresh</span>
      </button>
    </div>
  </div>
</div>
:::

</clr-row>

### Multiple Groups

Use when you want similar actions to be grouped together and separated from others.

::: do Lead with primary actions followed by secondary actions.

<div class="btn-group btn-primary" style="margin-right: 12px">
  <button class="btn">Create</button>
  <button class="btn">Edit</button>
</div>
<div class="btn-group btn-danger">
  <button class="btn">Delete</button>
  <button class="btn">Stop</button>
</div>
:::

::: dont Lead with secondary actions followed by primary actions.

<div class="btn-group btn-danger" style="margin-right: 12px">
  <button class="btn">Delete</button>
  <button class="btn">Stop</button>
</div>
<div class="btn-group btn-primary">
  <button class="btn">Create</button>
  <button class="btn">Edit</button>
</div>
:::

<!-- ## Placement -->

## Code & Examples

### Menu overflow

Use the clrInMenu input to determine if a button belongs in the overflow menu or not.

#### Default position

```html
<clr-button-group class="btn-primary">
  <clr-button>Create</clr-button>
  <clr-button>Favorite</clr-button>
  <clr-button [clrInMenu]="true">Assign</clr-button>
  <clr-button [clrInMenu]="true">Download</clr-button>
  <clr-button [clrInMenu]="true">Delete</clr-button>
</clr-button-group>
```

### Menu Position

```html
<clr-button-group class="btn-primary" [clrMenuPosition]="'bottom-right'">
  <clr-button>Create</clr-button>
  <clr-button>Favorite</clr-button>
  <clr-button [clrInMenu]="true">Assign</clr-button>
  <clr-button [clrInMenu]="true">Download</clr-button>
  <clr-button [clrInMenu]="true">Delete</clr-button>
</clr-button-group>
```

## Accessibility

If your icon button has no text, we recommend adding the **title="" attribute** to your icon buttons. This adds some
additional context for users unfamiliar with what action your icon button might produce. The text should reflect the
action.

```html
<div class="btn-group btn-primary btn-icon">
  <button class="btn">
    <clr-icon shape="check" title="Check"></clr-icon>
  </button>
  <button class="btn">
    <clr-icon shape="home" title="home"></clr-icon>
  </button>
  <button class="btn">
    <clr-icon shape="user" title="user"></clr-icon>
  </button>
</div>
```