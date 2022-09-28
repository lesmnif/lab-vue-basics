<script setup>
    const posts = [{title: "Hello", description:"I don't know", content:"Just some content here"},{title: "Second post", description:"Second post in the array", content:"As i just said this is the content of the second post"},{title: "Third Post", description:"Thid Post Info", content:"This is my third post content"}]
</script>

<template>
    <div>
        This is my Footer component :)
    </div>
    <div>
        This is my loop div
        <ul>
            <li v-for="post in posts" :key="post.title">
                This is my title: {{post.title}}, description: {{post.description}} and content: {{post.content}}
            </li>
        </ul>
    </div>
</template>

<style>

</style>