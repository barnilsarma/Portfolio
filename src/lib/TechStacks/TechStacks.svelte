<script>
    import styles from "./TechStacks.module.scss";
    import data from "../../../public/techstacks.json";
</script>

<main>
    <div class={styles.techstacks}>
        <h1>Currently Learning</h1>
        <div class={styles.innerParent}>
            {#each data as item}
                <div class={styles.item}>
                    <img src={item.logo} class={styles.logo} />
                    <div class={styles.hint}>
                        <h1 class={styles.name}>{item.name}</h1>
                        <h2 class={styles.status}>{item.status}</h2>
                    </div>
                </div>
            {/each}
        </div>
    </div>
</main>
