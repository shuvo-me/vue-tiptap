<script setup lang="ts">
import { EditorContent, useEditor } from '@tiptap/vue-3'
import StarterKit from '@tiptap/starter-kit';

 const editor = useEditor({
    content: "<p>I'm running Tiptap with Vue.js. 🎉</p>",
    extensions: [StarterKit],
    injectCSS: false,
    editorProps: {
      attributes: {
        class: 'editor-content',
      },
    },
  });
</script>

<template>
  <div class="editor-area">
     <editor-content :editor="editor" class="editor-content" />
  </div>
</template>
