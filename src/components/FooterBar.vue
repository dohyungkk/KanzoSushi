<template>
  <div class='background'>
    <div class='table'>
     <a class="openHour">
          OPENING HOUR
        </a>
    <table class="table-plain branch-hours">
      <tbody class="line">
        <tr class="Monday">
          <td>Monday: </td>
          <td>  11:00am - 9:00pm</td>
          <td></td>
        </tr>
      <tr class="Tuesday">
        <td>Tuesday: </td>
        <td>  11:00am - 9:00pm</td>
        <td></td>
      </tr>

      <tr class="Wednesday">
        <td>Wednesday: </td>
        <td>  11:00am - 9:00pm</td>
        <td></td>
      </tr>

      <tr class="Thursday">
        <td>Thursday: </td>
        <td>  11:00am - 9:30pm</td>
        <td></td>
      </tr>

      <tr class="Friday">
        <td>Friday: </td>
        <td>  11:00am - 9:30pm</td>
        <td></td>
      </tr>

      <tr class="Saturday">
        <td>Saturday: </td>
        <td>  11:00am - 9:30pm</td>
        <td></td>
      </tr>

      <tr class="Sunday">
        <td>Sunday: </td>
        <td>  11:00am - 9:30pm</td>
        <td></td>
      </tr>
  </tbody>
</table>
</div>
  <div class='other'>
    <a class='phoneAndAddress'> Phone Number and Address </a>
    <div class='phone'>
      778-379-3837 /
      778-379-3469
    </div>
    <div class='address'>
      2893 Grandview Hwy, Vancouver, BC, V5M 2E1
    </div>
  </div>
  </div>
</template>

<script>
export default {

}


</script>


<style scoped>

.openHour {
  color: #FFFF00;
}

.phone, .address {
  text-align: center;
}

.table {
  width: 50%;
  float: left;
  text-align: center;
}

.other {
  width: 50%;
  float: right;
  text-align: center;
}

.phoneAndAddress{
  text-align: center;
  margin-right: 150px;
}

a {
  font-family: 'TradeGothicW01-Extended', sans-serif;
    text-transform: uppercase;
    margin: 0;
    color: #FFFF00;
    font-size: 30px;
    margin-bottom: 20px;
}

.background {
  text-align: center;
}
table.table-plain,
table.table-plain td
{
    border: none !important;
    table-layout: auto;
    padding: .5rem;
    padding: 0;
    border-spacing: 0;
    font-family: "AvenirNextLTW01-Regular", sans-serif;
    font-size: 16;
    line-height: 1.3;
    color: #bcbcbc;
    margin-bottom: 20px;
    width: 100%;
    max-width: 377px;
}

table.table-plain td:first-child {
  text-align: center;
  font-weight: bold;
  width: 70%;

}

table.table-plain td:nth-child(2) {
  text-align: center;
}

#contact > div > div.table {
  background-color: #111111;
}

.other {
  background-color: white;
  font-family: "AvenirNextLTW01-Regular", sans-serif;
  font-size: 16;
  line-height: 1.3;
  color: #bcbcbc;
  text-align: center;
}

.line {
  text-align: center;
}

</style>
