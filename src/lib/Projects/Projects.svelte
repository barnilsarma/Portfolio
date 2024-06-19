<script>
    import styles from "./Projects.module.scss";
    import data from "../../../public/projects.json";
</script>

<main>
    <div class={styles.techstacks}>
        {#each data as item}
            <div class={styles.hint}>
                <h1>{item.name}</h1>
                <p>{item.desc}</p>
                <h2>{item.tasks}</h2>
                <h2>{item.tech}</h2>
                <a href={item.link}>Live Link</a>
                <a href={item.github}>Repo Link</a>
            </div>
        {/each}
    </div>
</main>
