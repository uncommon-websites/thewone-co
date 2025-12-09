<script lang="ts">
    export let color: "black" | "white" = "black";
</script>

<div class="flex items-center gap-2">
    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M7.5 6C5.01472 6 3 8.01472 3 10.5C3 12.9853 5.01472 15 7.5 15C8.65345 15 9.70584 14.5656 10.5 13.8467C11.2942 14.5656 12.3466 15 13.5 15C15.9853 15 18 12.9853 18 10.5C18 8.01472 15.9853 6 13.5 6C11.962 6 10.605 6.77285 9.75 7.9559C9.32843 6.79971 8.22325 6 7.5 6Z" fill={color} fill-opacity="0.8"/>
        <path d="M13.5 6C11.0147 6 9 8.01472 9 10.5C9 12.9853 11.0147 15 13.5 15C14.6534 15 15.7058 14.5656 16.5 13.8467C17.2942 14.5656 18.3466 15 19.5 15C21.9853 15 24 12.9853 24 10.5C24 8.01472 21.9853 6 19.5 6C17.962 6 16.605 6.77285 15.75 7.9559C15.3284 6.79971 14.2233 6 13.5 6Z" fill={color}/>
    </svg>
    <span class="text-xl font-bold tracking-tight" style="color: {color}">wone</span>
</div>
