<script>
    import styles from "./Activities.module.scss";
    import data from "../../../public/activities.json";
</script>

<main>
    <div class={styles.activities}>
        <h1 class={styles.heading}>College Activities</h1>
        <div class={styles.innerParent}>
            {#each data as item}
                <div class={styles.item}>
                    <h1 class={styles.activity}>{item.activity}</h1>
                    <p class={styles.desc}>{item.desc}</p>
                </div>
            {/each}
        </div>
    </div>
</main>
