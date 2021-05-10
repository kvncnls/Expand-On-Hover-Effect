<script>
    export let linkName = "link";
    export let src;
    export let content;
</script>

<a class="box box3" target="_blank" rel="noopener" href={src}>
    <h4>{linkName}</h4>
    <div>
        <p>{content}</p>
    </div>

    <svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M41.9999 7.5C41.9999 7.10218 41.8419 6.72064 41.5606 6.43934C41.2793 6.15804 40.8978 6 40.4999 6H22.4999C22.1021 6 21.7206 6.15804 21.4393 6.43934C21.158 6.72064 20.9999 7.10218 20.9999 7.5C20.9999 7.89782 21.158 8.27936 21.4393 8.56066C21.7206 8.84196 22.1021 9 22.4999 9H36.8789L6.43794 39.438C6.29848 39.5775 6.18785 39.743 6.11237 39.9252C6.03689 40.1075 5.99805 40.3028 5.99805 40.5C5.99805 40.6972 6.03689 40.8925 6.11237 41.0747C6.18785 41.257 6.29848 41.4225 6.43794 41.562C6.57741 41.7015 6.74297 41.8121 6.92519 41.8876C7.10741 41.963 7.30271 42.0019 7.49994 42.0019C7.69717 42.0019 7.89247 41.963 8.07469 41.8876C8.25691 41.8121 8.42248 41.7015 8.56194 41.562L38.9999 11.121V25.5C38.9999 25.8978 39.158 26.2794 39.4393 26.5607C39.7206 26.842 40.1021 27 40.4999 27C40.8978 27 41.2793 26.842 41.5606 26.5607C41.8419 26.2794 41.9999 25.8978 41.9999 25.5V7.5Z" fill="white"/>
        </svg>

</a>

<style lang="scss">
    @import url('https://fonts.googleapis.com/css2?family=Passion+One:wght@700&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300&display=swap');
.box {
    position: relative;
    font-family: 'Passion One', sans-serif;
    background-color: orangered;
    padding: 4rem 2rem;
    color: white;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    flex-grow: 1;
    flex-shrink: 1;
    flex-basis: 0;
    border: 1px solid white;
    overflow: hidden;
    cursor: pointer;
    transition: 300ms;
    margin: 1rem;
    svg {
        transition: 500ms;
        transform: rotate(90deg);
        opacity: 0;
    }
    div {
        position: absolute;
        transition: 300ms;
        height: 1.4rem;
        width: 50%;
        overflow: hidden;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        bottom: 4rem;
        p {
            font-family: 'Roboto', sans-serif;
            font-weight: bold;
            position: absolute;
            transition: 300ms;
            opacity: 1;
            font-size: 1.2rem;
            font-weight: 100;
            pointer-events: none;
            top: 50px;
        }
    }
    h4 {
        opacity: 1;
        transition: 250ms;
        text-transform: uppercase;
        font-size: 2.4rem;
    }
    @media (min-width: 768px) {
        &:hover {
        flex-grow: 2;
        background-color: whitesmoke;
        color: orangered;
            h4 {
                transform: scale(0.8) translateY(-3rem) translateX(-1rem);
            }
            div {
                width: 100%;
                p {
                opacity: 1;
                color: orangered;
                top: 0;
                }
            }

            svg {
                opacity: 1;
                transform: rotate(0);
                path {
                    fill: orangered;
                }
            }
        }
    }

    }
</style>

