# Component Library Index

Reference guide for all available components in the design system.

## Layout Components

### Frame

- Purpose: Container for grouping elements
- States: Default
- Sizes: Full-width, Fixed widths
- Specs: See layout guidelines

### Auto Layout

- Purpose: Responsive spacing and alignment
- Direction: Horizontal, Vertical
- Alignment: Various alignments
- Gap: 8px, 12px, 16px, 24px

### Grid

- Purpose: Align elements to grid
- Column counts: 4, 8, 12
- Gutter: 8px, 12px, 16px
- Responsive: Mobile, Tablet, Desktop

## Input Components

### Button

- **Variants**: Primary, Secondary, Tertiary, Danger
- **States**: Default, Hover, Active, Disabled, Loading
- **Sizes**: Small, Medium, Large, Extra Large
- **Features**: Icon support, text + icon, full-width
- **Usage**: CTAs, form submission, navigation

### Input Text Field

- **States**: Default, Focus, Filled, Error, Disabled
- **Features**: Placeholder, helper text, error message, prefix/suffix icons
- **Sizes**: Small, Medium, Large
- **Validation**: Success, warning, error

### Checkbox

- **States**: Unchecked, Checked, Indeterminate, Disabled
- **Sizes**: Small, Medium, Large
- **Label**: With/without label

### Radio Button

- **States**: Unselected, Selected, Disabled
- **Sizes**: Small, Medium, Large
- **Group**: Single or grouped options

### Select/Dropdown

- **States**: Default, Open, Disabled
- **Sizes**: Small, Medium, Large
- **Features**: Search, multi-select, custom styling

### Toggle Switch

- **States**: Off, On, Disabled
- **Sizes**: Small, Medium, Large
- **Labels**: With optional labels

### Textarea

- **States**: Default, Focus, Filled, Error, Disabled
- **Features**: Placeholder, helper text, character count, resizable
- **Sizes**: Small, Medium, Large

## Display Components

### Card

- **Variants**: Default, Elevated, Outlined
- **Features**: Header, content, footer, image, actions
- **States**: Default, Hover, Selected
- **Responsive**: Desktop, Tablet, Mobile

### Badge

- **Variants**: Primary, Secondary, Success, Warning, Error
- **Sizes**: Small, Medium, Large
- **Shapes**: Rounded, square, pill

### Chip

- **Variants**: Default, Closable, Selectable
- **States**: Default, Hover, Selected, Disabled
- **Sizes**: Small, Medium, Large

### Alert/Banner

- **Types**: Success, Info, Warning, Error
- **States**: Default, Dismissible
- **Icons**: Auto-generated based on type
- **Actions**: Optional action buttons

### Tooltip

- **Positions**: Top, Bottom, Left, Right
- **Trigger**: Hover, Click, Focus
- **Content**: Text, rich content

### Modal/Dialog

- **Types**: Confirmation, Alert, Form
- **Sizes**: Small, Medium, Large, Full-screen
- **Actions**: Primary, secondary, cancel

## Navigation Components

### Navigation Bar (Top)

- **Variants**: Default, Transparent, Sticky
- **Features**: Logo, menu items, search, user menu
- **Responsive**: Desktop, Mobile

### Sidebar Navigation

- **States**: Expanded, Collapsed
- **Features**: Icon + text, grouping, nested items
- **Active states**: Current page highlighting

### Breadcrumb

- **Styles**: Default, Icon variant
- **Separators**: / or >
- **Responsive**: Truncates on mobile

### Tabs

- **Styles**: Underline, Button, Pill
- **States**: Default, Active, Disabled
- **Responsive**: Scrollable or wrapped

### Pagination

- **Variants**: Numbered, Previous/Next, Infinite scroll
- **States**: Default, Active, Disabled
- **Features**: Jump to page, items per page

## Typography Styles

```
Heading/Large (H1) - 32px, Bold
Heading/Medium (H2) - 24px, Bold
Heading/Small (H3) - 18px, Bold

Body/Regular - 16px, Normal
Body/Small - 14px, Normal

Caption/Regular - 12px, Regular
Caption/Small - 11px, Regular

Label - 14px, Medium
Label/Small - 12px, Medium
```

## Icon Guidelines

- **Size**: 16px, 20px, 24px, 32px
- **Stroke**: 2px for consistency
- **Color**: Inherit from context
- **Usage**: Button icons, status indicators, navigation

## Using Components

### How to Use

1. Locate component in library file
2. Copy main component or drag instance
3. Customize properties (size, color, text)
4. Maintain component link for updates
5. Document any overrides

### Best Practices

- Always use instances, not copies
- Document overrides
- Use semantic variants
- Test all states
- Keep library updated

## Component Status

- 🟢 Ready to use
- 🟡 In development
- 🔴 Deprecated (don't use)
- ⚪ Planned

(Update status in actual library)
