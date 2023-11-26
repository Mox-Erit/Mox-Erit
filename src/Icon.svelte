<script>
    export let name;
    export let width = "1.5rem";
    export let height = "1.5rem";
    export let focusable = false;
    let icons = [
        {
          box: 24,
          name: "test1",
          svg: `<path fill="black" d="M3 5v14c0 1.103.897 2 2 2h14c1.103 0 2-.897 2-2V5c0-1.103-.897-2-2-2H5c-1.103 0-2 .897-2 2zm16.002 14H5V5h14l.002 14z"/><path fill="black" d="M15 12h2V7h-5v2h3zm-3 3H9v-3H7v5h5z"/>`
        },
        {
          box: 24,
          name: "test2",
          svg: `<path fill="black" d="M12 22c5.514 0 10-4.486 10-10S17.514 2 12 2S2 6.486 2 12s4.486 10 10 10zm0-18c4.411 0 8 3.589 8 8s-3.589 8-8 8s-8-3.589-8-8s3.589-8 8-8z"/><path fill="black" d="M19 12a7 7 0 0 0-7-7v14a7 7 0 0 0 7-7z"/>`
        }
    ];
    let displayIcon = icons.find((e) => e.name === name);
</script>

<svg
  class={$$props.class}
  {focusable}
  {width}
  {height}
  viewBox="0 0 {displayIcon.box} {displayIcon.box}">{@html displayIcon.svg}</svg>