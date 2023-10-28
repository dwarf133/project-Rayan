<template>
    <nav aria-label="Page navigation example">
        <ul class="pagination d-flex justify-content-end">
            <li class="pagination-item" v-for="link in links">
                <a v-show="parseInt(link.label)" class="page-link" :href="link['url']">
                    {{ link['label'] }}
                </a>
            </li>
        </ul>
    </nav>
</template>

<script>
    export default {
        props: ['links'],
        mounted() {
            console.log(this.links)
        },
        methods: {
            redirect(link) {
                console.log(link)
                let pageUrl = new URL(link.url);
                let page = pageUrl.searchParams.get('page');
                let currentUrl = new URL(window.location.href)

                currentUrl.searchParams.set('page', page)
                console.log(currentUrl.href);
            }
        }
    }
</script>

<style scoped>
    .pagination-item {
        background: #ffa343 !important;
        color: #000 !important;
    }
    .page-link {
        background: #ffa343 !important;
        color: #000 !important;
        border: 1px solid #202020;
    }
</style>
