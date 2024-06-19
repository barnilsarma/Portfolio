<script>
    import styles from "./TechStacks.module.scss";
    import data from "../../../public/techstacks.json";
</script>

<main>
    <div class={styles.techstacks}>
        {#each data as item}
            <img src={item.logo} />
            <div class={styles.hint}>
                <h1>{item.name}</h1>
                <h2>{item.status}</h2>
            </div>
        {/each}
    </div>
</main>
