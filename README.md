# python-embedded-shader

Adds syntax highlight support for shaders in python multiline strings in VS Code.

## Features

### Supported shader languages

* wgsl
* glsl
* hlsl
* metal

### Snippets

Provides snippets to create an embedded shader string, so you don't have to remember the syntax.

### Jinja templating

Jinja templates are syntax-highlighted. The tokens are rendered as keywords, and the content 
as string (shaders don't have/use string).

Unfortunately, this does *not* work for shaders embedded in Python strings. If you know how to
fix that I'd love to learn.

## Example

```py
for i in range(10):
    print(i)

shader = """//wgsl
    fn produceResult(vec2<f32> foo, f32 bar) -> vec2<f32> {
        return foo * bar;
    }
"""
````

## Notes

* You need to install syntax highlighting support for the shader languages separately. 
* This only provides syntax highlighting, no autocompletion or linting of your shaders.

