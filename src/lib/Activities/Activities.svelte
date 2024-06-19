<script>
    import styles from "./Activities.module.scss";
    import data from "../../../public/activities.json";
</script>

<main>
    <div class={styles.activities}>
        {#each data as item}
            <div class={styles.hint}>
                <h1>{item.activity}</h1>
                <h3>{item.desc}</h3>
            </div>
        {/each}
    </div>
</main>
