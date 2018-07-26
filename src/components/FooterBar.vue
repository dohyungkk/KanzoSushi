<template>
  <div class='background'>
    <div class='table'>
     <a class="openHour">
          OPENING HOUR
     </a>
    <table class="table-plain branch-hours">
      <tbody class="line">
        <tr class="Monday">
          <td>Monday to Sunday : 11:00am - 9:00pm</td>
        </tr>
  </tbody>
</table>
</div>
  <div class='other'>
    <a class='phoneAndAddress'> Phone Number and Address </a>
    <div class='phone'>
      604-568-4500 /
      604-558-4994
    </div>
    <div class='address'>
      82 Keefer Place (across International Village), Vancouver, BC, V6B 0C9
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
  color: #bcbcbc;
}

.phone, .address {
  text-align: center;
}

.table {
  width: 50%;
  float: left;
  max-width: 100%;
  margin-bottom: 1rem;
}

.other {
  width: 50%;
  float: right;
  text-align: center;
}

.phoneAndAddress{
  text-align: center;
}

a {
  	font-family: 'TradeGothicW01-Extended', sans-serif;
  	text-transform: uppercase;
    margin: 0;
    color: #bcbcbc;
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
    padding: 0;
    border-spacing: 0;
    font-family: "AvenirNextLTW01-Regular", sans-serif;
    line-height: 1.3;
    color: #bcbcbc;
    margin-bottom: 20px;
}

table.table-plain td:first-child {
  text-align: center;

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

td {
	    border: none;
    text-align: center;
}

</style>
