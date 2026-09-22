# Excursus: Jinja2 templates

This small digression covers *rudimentary* the syntax and semantics of the template engine. Since the template engine is very flexible, the configuration of the application may differ slightly from the code presented here in terms of delimiters and behavior of undefined values.

A `Jinja2` template is simply a text file. `Jinja2` can generate any text-based format (`HTML`, `XML`, `CSV`, `LATEX` and so on...). A `Jinja2` template does not require any specific extension such as `.html`, `.xml` or any other extension.

A template contains variables and/or expressions that are replaced with values ​​when the template is rendered.

A template also contains tags that control the logic of the template. The syntax here is heavily inspired by `Django` and `Python`.

There are different types of separators. The default `Jinja2` delimiters are configured as follows:

- `{% ... %}` → for (limited `Python`) statements
- `{{ ... }}` → for expressions to be displayed in the template output
- `{# ... #}` → for comments not included in the template output

Line instructions and comments are also possible, but do not have standard prefix characters and can only be used if the system (HA) specifies this.

***Template variables*** are defined by the *Dictionary* passed to the template. You can experiment with the variables in templates, provided that they are also passed by the application.

Variables can contain attributes or elements that can also be accessed. Which attributes a variable has depends largely on the application that is intended to provide this variable.

You can also use a dot (`.`) instead of the *standard* Python `__getitem__`-'subscript' syntax [ ] to gain access to a variable's attributes.

The following lines therefore do the same thing:

```yaml
{{ foo.bar }}  
{{ foo['bar'] }}
```

**Important**:
the outer double curly brackets `{{` are not part of the variable, but part of the `print` statement. If you want to access variables within tags, you cannot put them in curly brackets.

A minus sign (`-`) trims the corresponding object before (`{{-`, `{%-`) or after (`-}}`, `-%}`).

If a variable or attribute does not exist, the result will be an ***undefined*** value. What you can do with this type of value depends entirely on the configuration of the specific application:  
The default behavior is that after evaluation, when printing or iterating on an empty string, the process is immediately aborted and an error message is generated.
