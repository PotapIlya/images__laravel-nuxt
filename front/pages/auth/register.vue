<template>
  <div>

    <InputText
      label="test"
      placeholder="Test"


      @event="InputTextEvent"
    />

    <BtnInfo
      label="Отправить"

      @event="btnInfoClick"
    />
  </div>
</template>

<script>
  import BtnInfo from "../../components/base/buttons/info";
  import InputText from "../../components/base/inputs/text";
  export default {
    components: {
      BtnInfo,
      InputText
    },
    methods: {
      btnInfoClick(){
        console.log(12)
      },
      InputTextEvent(data){
        console.log(data)
      }
    }
  }
</script>
