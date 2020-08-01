# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `typescript > cast > arrow-async-parameter-as`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: true
	directives: Array []
	filename: "typescript/cast/arrow-async-parameter-as/input.ts"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "module"
	syntax: Array ["ts"]
	loc: Object {
		filename: "typescript/cast/arrow-async-parameter-as/input.ts"
		end: Object {
			column: 21
			index: 21
			line: 1
		}
		start: Object {
			column: 0
			index: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: MARKUP {parts: Array [RAW_MARKUP {value: "Unexpected type cast in parameter position"}]}
			}
			location: Object {
				filename: "typescript/cast/arrow-async-parameter-as/input.ts"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 13
					index: 13
					line: 1
				}
				start: Object {
					column: 7
					index: 7
					line: 1
				}
			}
		}
	]
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "typescript/cast/arrow-async-parameter-as/input.ts"
				end: Object {
					column: 21
					index: 21
					line: 1
				}
				start: Object {
					column: 0
					index: 0
					line: 1
				}
			}
			expression: JSArrowFunctionExpression {
				loc: Object {
					filename: "typescript/cast/arrow-async-parameter-as/input.ts"
					end: Object {
						column: 20
						index: 20
						line: 1
					}
					start: Object {
						column: 0
						index: 0
						line: 1
					}
				}
				body: JSBlockStatement {
					body: Array []
					directives: Array []
					loc: Object {
						filename: "typescript/cast/arrow-async-parameter-as/input.ts"
						end: Object {
							column: 20
							index: 20
							line: 1
						}
						start: Object {
							column: 18
							index: 18
							line: 1
						}
					}
				}
				head: JSFunctionHead {
					async: true
					hasHoistedVars: false
					rest: undefined
					returnType: undefined
					thisType: undefined
					loc: Object {
						filename: "typescript/cast/arrow-async-parameter-as/input.ts"
						end: Object {
							column: 17
							index: 17
							line: 1
						}
						start: Object {
							column: 0
							index: 0
							line: 1
						}
					}
					params: Array [
						JSBindingIdentifier {
							name: "INVALID_PLACEHOLDER"
							loc: Object {
								filename: "typescript/cast/arrow-async-parameter-as/input.ts"
								end: Object {
									column: 17
									index: 17
									line: 1
								}
								start: Object {
									column: 18
									index: 18
									line: 1
								}
							}
						}
					]
				}
			}
		}
	]
}
```

### `diagnostics`

```

 typescript/cast/arrow-async-parameter-as/input.ts:1:7 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Unexpected type cast in parameter position

    async (a as T) => {};
           ^^^^^^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```