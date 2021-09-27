<script>
    import MarkdownIt from 'markdown-it'
    import hljs from 'highlight.js'
    export let markdown = ''

    const md = new MarkdownIt({
        highlight: function (str, lang) {
            if(lang && hljs.getLanguage(lang)){
                try {
                    return hljs.highlight(lang, str).value
                }catch(e) {
                    console.error('Failed to highlight string')
                }
            }
            return ''
        },
    })
    const rendered = md.render(markdown)
    
</script>

<div>
    {@html rendered}
</div>
