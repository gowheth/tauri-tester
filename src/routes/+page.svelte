<script>
    import {Accordion, AccordionItem, Theme} from "carbon-components-svelte";

    let theme = "white";
</script>


<h1>Welcome to SvelteKit</h1>
<Theme bind:theme persist persistKey="__carbon-theme"
       render="select"
       select={{
    themes: ["white", "g10", "g80", "g90", "g100"],
    labelText: "Select a theme",
    inline: true,
  }}
/>

<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<Accordion>
    <AccordionItem title="Section 1" open> Content 1</AccordionItem>
    <AccordionItem title="Section 2"> Content 2</AccordionItem>
    <AccordionItem title="Section 3"> Content 3</AccordionItem>
</Accordion>

