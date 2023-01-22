<template>
    <section class="blogs">
        <div class="container">
            <div class="blogs-header">
                <h3>Latest from blog</h3>
                <a href="#"> see all</a>
            </div>
                    <div class="blogs-wrapper">
                        <div class="blog">
                            <div class="img-container">
                                <img src="@/assets/images/1.png" alt="blog">
                            </div>
                            <div class="blog-content">
                                <h3>The Easiest Way to Break</h3>
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation</p>
                            </div>
                        </div>
                        <div class="blog">
                            <div class="img-container">
                                <img src="@/assets/images/1.png" alt="blog">
                            </div>
                            <div class="blog-content">
                                <h3>The Easiest Way to Break</h3>
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation</p>
                            </div>
                        </div>
                        <div class="blog">
                            <div class="img-container">
                                <img src="@/assets/images/1.png" alt="blog">
                            </div>
                            <div class="blog-content">
                                <h3>The Easiest Way to Break</h3>
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation</p>
                            </div>
                        </div>
                    </div>
                </div>
    </section>
</template>

<script setup>

</script>

<style scoped>
.blogs .blogs-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 48px;
}

.blogs-header h3 {
    font-weight: 600;
    font-size: 22px;
    line-height: 25p;
}

.blogs-header a {
    font-weight: 500;
    font-size: 12px;
    line-height: 13px;
    opacity: 0.6;
    color: #121212;
}

.blogs-wrapper{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 30px;
}

.blog .blog-content{
    max-width: calc(100% - 48px);
    width: 100%;
    margin: auto;
    transform: translateY(-100px);
    background-color: #fff;
    padding: 24px 16px;
}

@media(max-width: 969px){
  .blogs-wrapper{
    grid-template-columns: 1fr 1fr;
  }
  .blog .blog-content{
    max-width: 100%;
    transform: translateY(0px);
  }
}
@media(max-width: 600px){
  .blogs-wrapper{
    grid-template-columns: 1fr ;
  }
  .blog .blog-content{
    padding: 10px 0px;
  }
}
</style>