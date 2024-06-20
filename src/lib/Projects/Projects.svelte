<script>
    import styles from "./Projects.module.scss";
    import data from "../../../public/projects.json";
</script>

<main>
    <div class={styles.projects}>
        <h1 class={styles.heading}>Projects ongoing/completed</h1>
        <div class={styles.innerParent}>
            {#each data as item}
                <div class={styles.item}>
                    <h1 class={styles.name}>{item.name}</h1>
                    <p class={styles.desc}>{item.desc}</p>
                    <p class={styles.tasks}>{item.tasks}</p>
                    <p class={styles.tech}>{item.tech}</p>
                    <div class={styles.linkCont}>
                        <a href={item.link} class={styles.link}>Live Link</a>
                        <a href={item.github} class={styles.github}>Repo Link</a
                        >
                    </div>
                </div>
            {/each}
        </div>
    </div>
</main>
