# Introduction

Maps in Elixir are the data structure for storing information in key-value pairs. In other languages, these might also be known as associative arrays (PHP), hashes (Perl 5, Raku), or dictionaries (Python).

Keys and values can be of any data type, but if the key is an atom we can use a shorthand syntax. Maps do not guarantee the order of their entries when accessed or returned.

## Literal forms

An empty map is simply declared with `%{}`. If we want to add items to a map literal, we can use two forms:

```elixir
# If the key is an atom:
%{atom_key: 1}

# If the key is a different type:
%{1 => :atom_value}

# You can even mix these if the atom form comes second:
%{"first_form" => :a, atom_form: :b}
```

While there is no canonical format, choose a consistent way to represent the key-value literal pairs.

## Map module functions

Elixir provides many functions for working with maps in the _Map module_. Some _Map module_ functions require an _anonymous_ function_ to be passed into the function to assist with the map transformation.
