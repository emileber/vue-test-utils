# html()

Returns HTML of wrapper DOM node as a string.

### Returns

(`String`): HTML of wrapper node

## Example

`Foo.vue`

```vue
<template lang="html">
    <div>
        <p>Foo</p>
    </div>
</template>

<script>
    export default {
      name: 'foo'
    }
</script>

```

`Foo.spec.js`

```js
import { mount } from 'vue-test-utils'
import { expect } from 'chai'
import Foo from './Foo.vue'

const wrapper = mount(Foo)
expect(wrapper.html()).to.equal('<div><p>Foo</p></div>')
```