<script>
export default {
    data() {
        return {
            jumboImg: "https://images.unsplash.com/photo-1540927764194-35c5c166886e?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTJ8fGNsYXNzeXxlbnwwfHwwfHw%3D&w=1000&q=80"
            
        }
    }
}
</script>

<template>
    <main>
        <div class="container">
            <div class="left">
                <h2>Hello & Welcome </h2>
                <h3>To Soul Night</h3>
                <p>"your favorite provider of soul music, whenever and wherever you want"</p>
            </div>
            <div class="right">
                <img :src="jumboImg" alt="">
            </div>
        </div>
    </main>
</template>

<style scoped>
main {
    height: calc(100vh - 58px);
}

.container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.left, .right {
    width: 48%;
}

.right {
    display: flex;
    justify-content: end;
}

.right img {
    width: 80%;
    border-radius: 10px;
    display: flex;
}

h2, h3 {
    font-size: 2.6rem;
    margin-bottom: 30px;
}

h3 {
    font-size: 2.4rem;
}

p {
    font-size: 1.2rem;
    margin: 10px 0;
}
</style>