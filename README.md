# python-embedded-shader

Adds syntax highlight support for python multiline shader strings in VS Code.

Supported shader languages:
* wgsl
* glsl

Also provides snippets to create an embedded shader string, so you don't have to remember the syntax.

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


## Status

Experimental.
