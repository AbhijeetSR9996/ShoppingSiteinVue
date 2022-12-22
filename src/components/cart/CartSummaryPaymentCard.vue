<template>
    <div class="cart-item-card">
        <h3>Cart Total: ${{cart_total.toFixed(2)}}</h3>
        <!-- <button class="view-product-button">Pay by Credit Card</button> 
        <button class="view-product-button">Pay by Dedit Card</button> -->

         <div class="button-container">
                <button class="add"> Debit Card</button>
                <button class="add"> Credit Card</button>
                <button class="add"> UPI </button>
                <button class="add"> Net Banking </button>
        </div>
        <h3>😊THANKYOU.VISIT AGAIN😊</h3>
    </div>
</template>

<script>
export default {
    computed: {
        cart_total() {
            return this.$store.getters.cartTotal
        }
    }
}
</script>
<style lang="scss">
.button-container {
        button {
            width:150px;
            border:none;
            padding: 10px;
            border-radius: 5px;
            margin: 0 5px 50px 5px;
            cursor: pointer;
        }
    }
.add {
    padding: 10px;
    background-color: rgb(79,160,187);
    border: none;
    color: white;
    font-weight: bold;
    font-size: 1.15rem;
    border-radius: 5px;
    cursor: pointer;
    }
</style>