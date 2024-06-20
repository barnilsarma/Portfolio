<script>
    import styles from "./Hero.module.scss";
</script>

<main>
    <div class={styles.hero}>
        <div class={styles.imgCont}>
            <img
                src="https://res.cloudinary.com/dcwqsevti/image/upload/v1694601618/ECS%20PHoto%20members/barnil.jpg"
                class={styles.photo}
            />
        </div>
        <h1 class={styles.myname}>Barnil Sarma</h1>
        <p class={styles.about}>
            Student | Dev | <span class={styles.procrast}>Pro-crastinator</span>
        </p>
    </div>
</main>
