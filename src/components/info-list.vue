<template>
    <section class="info-list">
        <ul>
            <li v-for="info in midInfo" :key="info.src">
                <info-preview  :info="info"/>
             </li>
        </ul>
    </section>
</template>
 
<script>
 import infoPreview from '../components/info-preview.vue'

export default {
 
name: '',
 data() {
return {
    midInfo: [
        {
            src: '/src/assets/images/icon-access-anywhere.svg',
            title: 'Access your files, anywhere',
            text: 'The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.'
        },
        {
            src: '/src/assets/images/icon-security.svg',
            title: 'Security you can trust',
            text: '2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.'

        },
        {
            src: '/src/assets/images/icon-collaboration.svg',
            title: 'Real-time collaboration',
            text: 'Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.'
        },
        {
            src: '/src/assets/images/icon-any-file.svg',
            title: 'Store any type of file',
            text: "Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared."
        }
    ]
};
 },
components: {
    infoPreview
}
};
</script>
 
<style>
 
</style>