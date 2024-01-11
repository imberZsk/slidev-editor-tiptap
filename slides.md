---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shikiji
lineNumbers: false
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
transition: slide-left
title: Welcome to Slidev
mdc: true
---

# 编辑器技术选型

Editor Technology Selection

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---

# 目标和需求

细化技术选型各方面需要考虑的事情

- 🤭 **编辑器定位** - 先了解各种编辑器定位，为后续选型做参考。
- 🎨 **编辑器优缺点** - 对比各种编辑器优缺点，选出不适合需求的编辑器。
- 🤹 **文档和社区支持** - 评估技术的文档质量和社区支持。良好的文档和活跃的社区可以提供有关技术的帮助、解决问题和分享最佳实践。
- 🎥 **性能和可靠性** - 考虑编辑器的性能和可靠性要求。对于大型项目或需要高度稳定性的场景，可能需要选择经过良好测试并具有高性能的编辑器技术。
- 🧑‍💻 **插件和扩展性** - 考虑编辑器的插件和扩展能力。一个好的编辑器应该能够支持自定义插件和扩展，以满足特定的需求。
- 📤 **可视化和用户体验** - 用户体验至关重要，需要考虑编辑器的可视化效果和用户界面。分析评估编辑器的样式定制性、交互性和用户友好性。
- 🛠 **趋势和前景** - 了解当前市场上的编辑器技术趋势和前景。考虑技术的发展方向、社区活跃程度以及商业支持等因素。

<br>
<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 编辑器定位

数据来源于 GitHub 对应编辑器项目 About

| 名称      | About                                                                      |
| --------- | -------------------------------------------------------------------------- |
| Quill     | Quill 是一款专为兼容性和可扩展性而构建的现代所见即所得编辑器               |
| Draft.js  | 用于构建文本编辑器的 React 框架。                                          |
| lexical   | Lexical 是一个可扩展的文本编辑器框架，可提供出色的可靠性、可访问性和性能。 |
| Slate.js  | 用于构建富文本编辑器的完全可定制的框架。 （目前处于测试阶段。）            |
| editor.js | 具有通用 JSON 输出的免费块式编辑器                                         |
| plate     | React 的富文本编辑器                                                       |
| tiptap    | 适合 web 的 CMS 无头编辑器框架                                             |

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 编辑器缺点

数据来源于 [推荐十个优秀的富文本编辑器](https://juejin.cn/post/7201883287937990712?searchId=202312141611152B252BE78D887447895C#heading-4)

| 名称      | 缺点                                                                              |
| --------- | --------------------------------------------------------------------------------- |
| Quill     | quill 一直卡在 2.0@dev 中, 后面的升级都需要自己来维护，后续开发新功能会花些精力。 |
| Draft.js  | 后期不再新增任何功能，官方推荐了新的库（lexical），有被放弃的危险                 |
| lexical   | 更新迭代很快，有些功能不一定完善，demo UI 不太好看                                |
| Slate.js  | 不是开箱即用，需要二次开发                                                        |
| editor.js | 许多功能需要引入插件或者自定义实现                                                |
| plate     | 虽然已有很多插件，但自定义插件拓展不太清晰方便                                    |
| tiptap    | Pro 插件需要收费                                                                  |

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# 文档和社区支持

tiptap 有令人震惊的超多 demo 和拓展插件，而且文档写得非常清晰，虽然大约有 10 个插件是收费的，但可以参考开源项目来自己实现。在它的云后台还能看到一些编辑器数据。

<div grid="~ cols-2 gap-2" m="-t-2">

```yaml
---
Examples
---
```

```yaml
---
Extensions
---
```

<img border="rounded" src="/2.jpg">
<img border="rounded" src="/1.jpg">

</div>

Read more about [Examples](https://tiptap.dev/docs/editor/examples/default) and
Read more about [Extensions](https://sli.dev/themes/gallery.html).

<!-- Use code snippets and get the highlighting directly![^1]

```ts {all|2|1-6|9|all}
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: User) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

<arrow v-click="3" x1="400" y1="420" x2="230" y2="330" color="#564" width="3" arrowSize="1" />

[^1]: [Learn More](https://sli.dev/guide/syntax.html#line-highlighting)

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style> -->

---

# 性能和可靠性(tiptap)

数据来源于 [npm.dev.tech](https://npm.devtool.tech/tiptap)

<img border="rounded" src="/3.jpg">

---

# 性能和可靠性(plate.js)

数据来源于 [npm.dev.tech](https://npm.devtool.tech/@udecode/plate-common)

<img border="rounded" src="/4.jpg">

---

# 性能和可靠性(editor.js)

数据来源于 [npm.dev.tech](https://npm.devtool.tech/@editorjs/editorjs)

<img border="rounded" src="/5.jpg">

---

# 性能和可靠性-综合对比

数据来源于 [npm-compare](https://npm-compare.com/@tiptap/react,@udecode/plate-common,@editorjs/editorjs)

<img border="rounded" src="/6.jpg">

---

# 可视化和用户体验

先理解一个词 Headless：没有提供用户界面，您可以完全自由地构建您想要的任何界面。无需覆盖任何类、使用 !important 或其他技巧，只需在您习惯的设置中编写您喜欢的任何内容（只提供逻辑，不提供 UI 界面）

<div grid="~ cols-2 gap-2" m="-t-2">

```md
这是一个引用和一个加粗功能

它们的样式完全由我们的代码控制，tiptap 不会附加样式
如果是 wangeditor，它的图标都无法修改，只能通过 CSS 覆盖

其他还有很多细节，这里列举一些：

1、提升用户体验的光标
```

<img border="rounded" src="/7.jpg">

</div>

---

# 趋势和前景

有超过 20,000 家企业在使用 Tiptap，260w$投资

参考 [开源富文本编辑器 wangEditor 暂停维护 （但仍可继续使用）](https://juejin.cn/post/7272735633458413602?searchId=202401111515277FCC4B9364849CA012E1)

参考 [github Sponsors](https://github.com/ueberdosis/tiptap?tab=readme-ov-file#sponsors-)

参考 [tiptap](https://tiptap.dev/blog/insights)

### 站在巨人的肩膀

- [novel](https://github.com/steven-tey/novel)，在线 [Demo](https://novel.sh/) 地址
- [tittap template](https://github.com/ueberdosis/tiptap-templates)，在线 [Demo](https://templates.tiptap.dev/NTFHDfnbFd) 地址
- [BlockNote](https://github.com/TypeCellOS/BlockNote)
- [think](https://github.com/fantasticit/think)

---

# 插件和扩展性

这里演示调研进展、一个自定义投票插件、和演示一下所见即所得

http://172.29.240.111:3000/editor

---

# 一些心得

1. `tiptap` 插件使用清晰，插件开箱即用，能减少大量开发时间。

2. 它想法很好，它有个入门套件，叫，可以通过 `starterKit` 一个插件就能把常用功能覆盖掉，而且也支持修改这些常用功能，减少了很大一部分代码。

3. 封装的一些方法和拓展，符合函数式编程思想，比如操作按钮支持 `bold` 功能，可以去看它的 `example`，或者去看它拓展插件，可以快速实现该功能，而且仅仅是函数调用的方式（清晰优雅）。

4. 一些细节也到位，比如 `focus`，不阻止用户输入，自定义样式 `headless`，自定义输出等，协同也支持，不过用不上，编辑器光标。

---

# 展望

<div class="m-auto w-full text-center absolute top-[50%] left-0">思考要做出一个什么样的编辑器？</div>
