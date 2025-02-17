---
id: 'Truncate'
beta: true
section: components
cssPrefix: pf-c-truncate
---

## Examples

### Notes
The truncate component contains two child elements, `.pf-c-truncate__start` and `.pf-c-truncate__end`. If both `start` and `end` are present within `.pf-c-truncate`, trucation will occur in the middle of the string. If only `.pf-c-truncate__start` is present, truncation will occur at the end of the string. If only `.pf-c-truncate__end` is present, truncation will occur at the beginning of the string. A `.pf-c-popover` will be automatically applied to the PatternFly React implementation. `&lrm;` must be included at the end of string to denote the ending punctuation mark. Otherwise it will occur and the beggining of truncation for a `pf-c-truncate__end` element.

### Default
```hbs
<div style="width: 220px; resize: horizontal; overflow: auto;">
  {{#> truncate truncate--id="default-truncation-example"}}
    {{> truncate-start truncate-start--text="Vestibulum interdum risus et enim faucibus, sit amet molestie est accumsan."}}
  {{/truncate}}
</div>
```

### Middle
```hbs
<div style="width: 226px; resize: horizontal; overflow: auto;">
  {{#> truncate truncate--id="middle-of-line-truncation-example"}}
    {{> truncate-start truncate-start--text="redhat_logo_black_and_white_reversed_"}}
    {{> truncate-end truncate-end--text="simple_with_fedora_container.zip"}}
  {{/truncate}}
</div>
```

### Start
```hbs
<div style="width: 220px; resize: horizontal; overflow: auto;">
  {{#> truncate truncate--id="start-truncation-example"}}
    {{> truncate-end truncate-end--text="Vestibulum interdum risus et enim faucibus, sit amet molestie est accumsan.&lrm;"}}
  {{/truncate}}
</div>
```

## Documentation

### Usage

| Class | Applied | Outcome |
| -- | -- | -- |
| `.pf-c-truncate` | `<span>` | Initiates the truncate component. |
| `.pf-c-truncate__start` | `<span>` | Defines the truncate component starting text. |
| `.pf-c-truncate__end` | `<span>` | Defines the truncate component ending text. |
| `.pf-c-truncate__text` | `<span>` | Defines the truncate component text. |
