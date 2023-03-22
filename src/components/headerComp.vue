<script>
export default {
    data() {
        return {
            title: "Soul Night",
            navBarOne: "Services",
            navBarTwo: "Gallery",
            navBarThree: "Contact",
            login: "Login"
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="title">
            <h1>{{ title }}</h1>
        </div>
        <nav>
            <ul>
                <li>
                    <a href="#">
                        {{ navBarOne }}
                    </a>
                </li>
                <li>
                    <a href="#">
                        {{ navBarTwo }}
                    </a>
                </li>
                <li>
                    <a href="#">
                        {{ navBarThree }}
                    </a>
                </li>
            </ul>
        </nav>
        <div class="login">
            <button>{{ login }}</button>
        </div>
        </div>
    </header>
</template>

<style scoped>
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header h1 {
    font-size: 1.5rem;
}

header ul {
    display: flex;
}

header li {
    padding: 10px;
    margin: 10px;
    position: relative;
}

header a::after {
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 3px;
        background-color: #f7ead1;
        transform: scaleX(0);
        transform-origin: bottom left;
        transition: transform 0.3s;
    }

header a:hover::after {
            transform: scaleX(1);
    }

header li a {
    color: #f7ead1;
}

header button {
    padding: 7px 14px;
    border: 0;
    border-radius: 5px;
    font-weight: bold;
    background-color: brown;
    color: #f7ead1;
}

header button:hover {
    transform: translateY(-6px);
    transition: ease .40s;
}
</style>