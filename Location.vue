<template>
    <div>
        <div></div>
        <div class="google-map">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1954.5993627070513!2d104.88802510012405!3d11.537597704679863!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31095056db4df965%3A0xf3e87c74061a81e6!2sNational%20Institute%20of%20Business!5e0!3m2!1sen!2skh!4v1722873022410!5m2!1sen!2skh" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
    </div>
</template>

<style scoped>
    .google-map {
     padding-bottom: 50%;
     position: relative;
}

.google-map iframe {
     height: 100%;
     width: 100%;
     left: 0;
     top: 0;
     position: absolute;
}
</style>