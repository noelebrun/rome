# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `typescript > import > equals`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	diagnostics: Array []
	directives: Array []
	filename: "typescript/import/equals/input.ts"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "module"
	syntax: Array ["ts"]
	loc: Object {
		filename: "typescript/import/equals/input.ts"
		end: Object {
			column: 0
			line: 2
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	body: Array [
		TSImportEqualsDeclaration {
			id: JSBindingIdentifier {
				name: "A"
				loc: Object {
					filename: "typescript/import/equals/input.ts"
					identifierName: "A"
					end: Object {
						column: 8
						line: 1
					}
					start: Object {
						column: 7
						line: 1
					}
				}
			}
			isExport: false
			loc: Object {
				filename: "typescript/import/equals/input.ts"
				end: Object {
					column: 15
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			moduleReference: TSQualifiedName {
				loc: Object {
					filename: "typescript/import/equals/input.ts"
					end: Object {
						column: 14
						line: 1
					}
					start: Object {
						column: 11
						line: 1
					}
				}
				left: JSReferenceIdentifier {
					name: "B"
					loc: Object {
						filename: "typescript/import/equals/input.ts"
						identifierName: "B"
						end: Object {
							column: 12
							line: 1
						}
						start: Object {
							column: 11
							line: 1
						}
					}
				}
				right: JSIdentifier {
					name: "C"
					loc: Object {
						filename: "typescript/import/equals/input.ts"
						identifierName: "C"
						end: Object {
							column: 14
							line: 1
						}
						start: Object {
							column: 13
							line: 1
						}
					}
				}
			}
		}
	]
}
```

### `diagnostics`

```
✔ No known problems!

```
