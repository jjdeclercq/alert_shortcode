# Alert Extension For Quarto

A framework for creating Quarto callouts using YAML. Additional inputs allow for tracking and logging issues throughout the lifespan of the document. 

## Installing

In a terminal window, navigate to the working directory of the project for which you want to use the shortcode, then paste in this command:

```bash
quarto add jjdeclercq/alert_shortcode
```

This will install the extension under the `_extensions` subdirectory.
If you're using version control, you will want to check in this directory.

## Using

YAML structure for shortcode arguments:

- [`alert_name:`] Each alert must have a unique name   
  - `title:` The title of the callout (optional)
  - `type:` The standard callout types: `warning`, `tip`, `note`, `important`, `caution`
  - `content:` The text to include in the callout
  - `icon:` `true`/`false` - Include the callout icon (defaults to `true`)
  - `collapse:` `true`/`false` - Whether of not the callout is collapsed (defaults to `false`)
  - `date_created:` Date alert first created (Optional)
  - `resolved:` `yes`/`no` - Whether or not the alert is resolved (defaults to `no`)
  - `date_resolved:` Date alert resolved (Optional)
  - `resolution:` A description of how the alert was resolved (Optional)
  - `include_extras:` `yes`/`no` - Whether or not to inlcude alert metadata (resolution status, dates) in the callout (defaults to `no`)

## Example

Here is the source code for a minimal example: [example.qmd](example.qmd).

