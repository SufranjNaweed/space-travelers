<template>
    <form id="newsletter" class="mx-auto" @submit="checkForm">
        <input type="text" name="email" id="email" placeholder="email tony.stark@avengers.tech">
        <input type="submit" value="SUBMIT">
    </form>
</template>

<script>
export default {
  name: 'Newsletter',
  methods: {
    checkForm (e) {
      e.preventDefault()
      console.log('Validate Forms')
    }
  }
}
</script>

<style lang="scss">
$ctaColor : #F9A826;
#newsletter{
    position: relative;
    z-index: 10;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 10px auto;
    #email{
        font-size: 12px;
        padding: 10px;
        height: 55px;
        max-width: 250px;
        width: 100%;
        border-top-left-radius: 8px;
        border-bottom-left-radius: 8px;
        &::placeholder{
            letter-spacing: 4px;
            max-width: 310px;
        }
        @media (min-width: 640px) {
            font-size: 22px;
            max-width: 510px;
        }
    }
    input[type="submit"]{
        cursor: pointer;
        border: solid 1px #121212;
        letter-spacing: 3px;
        font-weight: 700;
        font-size: 22px;
        max-width: 150px;
        width: 100%;
        height: 55px;
        color: #fff;
        background-color: $ctaColor;
        border-color: $ctaColor;
        border-top-right-radius: 8px;
        border-bottom-right-radius: 8px;
    }
}
</style>
