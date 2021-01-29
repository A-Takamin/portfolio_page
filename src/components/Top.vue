<template>
    <section id="top" class="top-section">
        <div class="container">
            <div class="row row-eq-height">
                <div class="col-md-8 top-img-wrapper">
                    <img v-bind:src="image">
                </div>
                <div class="col-md-4 top-name-wrapper">
                    <h1>Aki<br>Takami</h1>
                    <p>Promising Programmer</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Top',
    data() {
        return {
            image: '/samahika3.jpg'
        }
    }
}
</script>

<style scoped>
.top-img-wrapper{
  text-align: center;
  height: 500px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.top-img-wrapper img{
  max-width: 100%;
  height:auto;
  border-radius: 10px;
}

.top-name-wrapper{
  padding-top: 100px;
  padding-left: 50px;
}

.top-name-wrapper h1{
  font-size: 60px;
}

@media (max-width: 1024px){
  .top-img-wrapper{
    display: none;
  }

  .top-name-wrapper{
    padding: 0px;
    text-align: center;
  }
}
</style>