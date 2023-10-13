# Example Markdown with PUML
Set `plantuml:{filename}` as a fence information. `filename` is used as the file name of generated diagrams. In the following case, `md-sample-sequence.svg` is created.
`filename` is required.

```plantuml:md-sample-sequence
@startuml
actor Foo123
boundary Foo2
control Foo3
entity Foo4
database Foo5
collections Foo6
Foo1 -> Foo2 : To boundary
Foo1 -> Foo3 : To control
Foo1 -> Foo4 : To entity
Foo1 -> Foo5 : To database
Foo1 -> Foo6 : To collections
@enduml
```

![](./render/md-sample-sequence.svg)

# Sample 2 for using PUML
To host just plantuml, without showing the markup itself, you could keep the puml file separately, and just refer to the generated svg file like a regular image file. See below:

![](./render/json.svg)
