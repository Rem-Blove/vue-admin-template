<!-- @format -->

<template>
  <div>
    <div class="card-header">
      <span>{{ title }}</span>
      <svg
        t="1686645965633"
        class="icon"
        viewBox="0 0 1024 1024"
        version="1.1"
        xmlns="http://www.w3.org/2000/svg"
        p-id="1468"
        width="16"
        height="16"
      >
        <path
          d="M512 97.52381c228.912762 0 414.47619 185.563429 414.47619 414.47619s-185.563429 414.47619-414.47619 414.47619S97.52381 740.912762 97.52381 512 283.087238 97.52381 512 97.52381z m0 73.142857C323.486476 170.666667 170.666667 323.486476 170.666667 512s152.81981 341.333333 341.333333 341.333333 341.333333-152.81981 341.333333-341.333333S700.513524 170.666667 512 170.666667z m36.571429 268.190476v292.571428h-73.142858V438.857143h73.142858z m0-121.904762v73.142857h-73.142858v-73.142857h73.142858z"
          p-id="1469"
        />
      </svg>
    </div>
    <div class="card-content">
      <p>{{ count }}</p>
    </div>
    <div class="card-charts">
      <slot name="charts" />
    </div>
    <div class="card-footer">
      <slot name="footer" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Detail',
  props: ['title', 'count']
}
</script>

<style scoped>
.card-header{
  display: flex;
  justify-content: space-between;
  color: #999;
  font-size: 14px;
}
.card-content{
  font-size: 22px;
}
.card-charts{
  height: 50px;
  padding-bottom: 5px;
  border-bottom: 1px solid #ccc;

}
.card-footer{
  margin-top: 10px;
}
</style>
