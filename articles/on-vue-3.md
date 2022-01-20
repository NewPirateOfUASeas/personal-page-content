---
title: Why I'm worried about Vue future
description: On future of vue.js
img: https://upload.wikimedia.org/wikipedia/commons/9/95/Vue.js_Logo_2.svg
long: true
---
# Introduction
For those unaware - [Vue.js is one of the 3 most popular javascript frameworks.](https://gist.github.com/tkrotoff/b1caa4c3a185629299ec234d2314e190). 
It would be right to start with why I care about the subject: I love using vue, it delivers an awesome DX for a small teams, and it's my favorite JS framework. With this beinig said, let's dive straight into subject.

## Vue 3
I'll start with the positives: Vue 3 removed [filters](https://v3.vuejs.org/guide/migration/filters.html), various sources also report that performance has been [drastically improved](https://geckodynamics.com/blog/vue2-vs-vue3) referring to this [document](https://docs.google.com/spreadsheets/d/1VJFx-kQ4KjJmnpDXIEaig-cVAAJtpIGLZNbv3Lr4CR0/edit#gid=0). I couldn't verify if this document is legit though. But I think DX has been greatly improved for sure, especially since Typescript compatibility has been improved.

## Drawbacks

### Composition-API
While i have no problem with composition API itself, i do think that it just makes things more complicated. Unlike React, which stated that, in fact, they're keeping class components for the sake of backward-compatibility, but for new components u should use hooks:
> > #### Should I use Hooks, classes, or a mix of both?
> When you’re ready, we’d encourage you to start trying Hooks in new components you write. Make sure everyone on your team is on board with using them and familiar with this documentation. We don’t recommend rewriting your existing classes to Hooks unless you planned to rewrite them anyway (e.g. to fix bugs).
Source: https://reactjs.org/docs/hooks-faq.html

The Vue team goes the other way and claims that the Composition-API is purely *additive*:
> **The composition API is additive**, it’s a new feature, but it doesn’t and will not replace the good ole “Options API” you know and love from Vue 1 and 2. Just consider this new API as another tool in your toolbox that may come in handy in certain situations that feel a little clumsy to solve with the Options API. -- [Thorsten Lünborg](https://github.com/LinusBorg)
Source: https://www.vuemastery.com/blog/vue-3-data-down-events-up/

> I think Ari brings up an excellent point that when composition API just hasn't quite clicked like, “Why would I need that? The options API is working for me.” That's great. That means you don't need it. I think that's really important to emphasize here is that this is not something you need to go and rewrite your app in. It's a technique that when you have this problem that you need, just like in Damien’s button example, there's a reason why a component that's props heavy becomes very difficult to maintain, because now you basically have to read documentation to use it. Why slots becomes an incredible asset and tool to solve a problem of too many props. Similarly, the composition API is not like, drop the options do composition. **It's an additive thing that when you have a problem that it can solve, it's really great for that.** -- [Ben Hong](https://www.bencodezen.io/)
Source: https://enjoythevue.io/episodes/48/

> Without trying to argue, just out of interest: why Vue is is less dev happiness than Vue 2? Options API didn't change that much, and the **Composition API is purely additive**. Why do you find Vue 3 less enjoyable than version 2? --[Natalia Tepluhina](https://www.nataliatepluhina.com/)
Source: https://twitter.com/N_Tepluhina/status/1349429774729572352

This fact makes it unclear whether you should use Options-API or Composition-API in any given situation. This also means that you should be familiar with both APIs as they are accepted by popular libraries like [Vuelidate](https://vuelidate.js.org/) or [Vuetify](https://vuetifyjs.com/en/). In other words, there is no such thing as an *additive* API.

### Typescript
While it is really important to have strong types, especially in large projects, a structural type system is not enough today when web applications can be used in important things like [healthcare](https://www.researchgate.net/publication/251225200_Web-Based_Applications_in_Healthcare) (which, firstly, is a big mistake, but this is a completely different topic), and the chosen typing system can even be [cause of death (RU)](https://youtu.be/jnSHRPCTFPc?t=727). The problem is that Vue only officially supports typescript, and [Rescript/BuckleScript](https://rescript-lang.org/) or [Hegel](https://hegel.js.org/) isn't even an option. On the other hand, React, being simple in nature, is [easy to use with Rescript](https://rescript-lang.org/docs/react/latest/introduction).

### Mixins
Fortunately or not, mixins are getting less popular thanks to Composition-API. However, mixins are a real pain to work with. Don't believe me? Try to understand how this component works - https://github.com/bootstrap-vue/bootstrap-vue/blob/dev/src/components/carousel/carousel.js 
