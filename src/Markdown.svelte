<script>
    import MarkdownIt from 'markdown-it'
    import hljs from 'highlight.js'
    import 'highlight.js/styles/github-dark.css'
    export let markdown = ''

    var md = new MarkdownIt({
        highlight: function (str, lang) {
        if (lang && hljs.getLanguage(lang)) {
            try {
                return '<pre class="hljs"><code>' +
               hljs.highlight(str, { language: lang, ignoreIllegals: true }).value +
                   '</code></pre>';
            } catch (__) {}
        }
        return '<pre class="hljs"><code>' + md.utils.escapeHtml(str) + '</code></pre>';
  }
});

    const rendered = md.render(markdown)
    
</script>

<div class="md">
    {@html rendered}
</div>