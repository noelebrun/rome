# `noCatchAssign.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romejs/compiler/lint/rules/js/noCatchAssign.test.ts --update-snapshots` to update.

## `no exception assign`

### `0`

```
✔ No known problems!

```

### `0: formatted`

```
try {
} catch (e) {
	three = 2 + 1;
}

```

### `1`

```
✔ No known problems!

```

### `1: formatted`

```
try {
} catch ({e}) {
	this.something = 2;
}

```

### `2`

```
✔ No known problems!

```

### `2: formatted`

```
function foo() {
	try {
	} catch (e) {
		return false;
	}
}

```

### `3`

```

 unknown:1:23 lint/js/noCatchAssign ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Do not reassign catch parameters.

    try { } catch (e) { e; e = 10; }
                           ^

  ℹ Use a local variable instead.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `3: formatted`

```
try {
} catch (e) {
	e;
	e = 10;
}

```

### `4`

```

 unknown:1:42 lint/js/noCatchAssign ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Do not reassign catch parameters.

    try { } catch (ex) { console.log('test'); ex = 10; }
                                              ^^

  ℹ Use a local variable instead.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `4: formatted`

```
try {
} catch (ex) {
	console.log("test");
	ex = 10;
}

```

### `5`

```

 unknown:1:22 lint/js/noCatchAssign ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Do not reassign catch parameters.

    try { } catch (ex) { [ex, test] = []; }
                          ^^

  ℹ Use a local variable instead.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `5: formatted`

```
try {
} catch (ex) {
	[ex, test] = [];
}

```

### `6`

```

 unknown:1:34 lint/js/noCatchAssign ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Do not reassign catch parameters.

    try { } catch ({message, name}) { message = 'test'; name = 10; }
                                      ^^^^^^^

  ℹ Use a local variable instead.

 unknown:1:52 lint/js/noCatchAssign ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Do not reassign catch parameters.

    try { } catch ({message, name}) { message = 'test'; name = 10; }
                                                        ^^^^

  ℹ Use a local variable instead.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 2 problems

```

### `6: formatted`

```
try {
} catch ({message, name}) {
	message = "test";
	name = 10;
}

```

### `7`

```

 unknown:1:26 lint/js/noCatchAssign ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Do not reassign catch parameters.

    try { } catch (ex) { ({x: ex = 0} = {}); }
                              ^^

  ℹ Use a local variable instead.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `7: formatted`

```
try {
} catch (ex) {
	({x: ex = 0} = {});
}

```

### `8`

```

 unknown:1:37 lint/js/noCatchAssign ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Do not reassign catch parameters.

    try { } catch (ex) { let a; ({x: a = ex = 0} = {}); }
                                         ^^

  ℹ Use a local variable instead.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `8: formatted`

```
try {
} catch (ex) {
	let a;
	({x: a = ex = 0} = {});
}

```