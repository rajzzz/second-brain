**Document Type Definiton** is a schema language that defines the structure, allowed elements, attribute lists and order of elements in an [[XML]] document.

It ensures the [[XML]] is **valid** and not just well formed.

## Types:
1. Internal: Defined within the XML file.
2. External: stored in a seperate `.dtd` file and linked to XML.

``` XML
<!DOCTYPE employee [
	<!ELEMENT employee(id, name, department)>
	<!ELEMENT id (#PCDATA)>
	<!ELEMENT name (#PCDATA)>
	<!ELEMENT department (#PCDATA)>
]>
<employee>
	<id>101</id>
	<name>Raj</name>
	<department>Social Media</department>
</employee>
```

## Limitations:
1. Not written in XML.
2. Limited data types (like [[PCDATA]] and ID).
3. No support for namespaces or strong typing.