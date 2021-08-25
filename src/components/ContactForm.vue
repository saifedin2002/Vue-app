<template>
    <form action="" class="contact" method="post">
        <input type="text" name="name" placeholder="name..." />
        <input type="email" name="email" placeholder="email..." />
        <input type="password" name="password" placeholder="password" />
        <input type="submit" value="submit" class="submait" />
    </form>
</template>

<script>
export default {
    name: "CotactForm",
};
</script>

<style lang="scss" scoped>
.contact {
    height: 900px;
    display: block;
    overflow: hidden;
    margin: 0px auto;
    background-color: #444;
    input {
        width: 80%;
        margin: 0 auto;
        height: 100px;
        border: none;
        border-bottom: 5px solid #fff;
        color: #fff;
        background-color: #444;
        padding: 20px;
        display: block;
    }
    .submait {
        width: 200px;
        border: 5px solid #fff;
        top: 50px;
        margin-top: 50px;
        font-size: 30px;
        &:hover {
            background-color: #fff;
            color: #444;
        }
    }
}
</style>
