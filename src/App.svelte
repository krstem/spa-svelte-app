<script>
</script>

<style>
  /* Styles for the product checkout form */

  div.main-div {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
  }

  h1 {
      text-align: center;
      color: #333;
  }

  form {
      max-width: 400px;
      margin: 0 auto;
  }

  div {
      margin-bottom: 10px;
  }

  label {
      display: block;
      font-weight: bold;
      margin-bottom: 5px;
  }

  input[type="text"],
  input[type="email"],
  textarea {
      width: 100%;
      padding: 8px;
      border: 1px solid #ccc;
      border-radius: 4px;
  }

  input[type="submit"] {
      padding: 10px 20px;
      background-color: #333;
      color: #fff;
      border: none;
      border-radius: 4px;
      cursor: pointer;
  }

  input[type="submit"]:hover {
      background-color: #555;
  }

</style>

<section>
    <div class='main-div'>
        <h1>Product Checkout</h1>
                <form action="/process_payment" method="POST">
                    <div>
                        <label for="name">Name:</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div>
                        <label for="email">Email:</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div>
                        <label for="address">Address:</label>
                        <textarea id="address" name="address" required></textarea>
                    </div>
                    <div>
                        <label for="card_number">Card Number:</label>
                        <input type="text" id="card_number" name="card_number" required>
                    </div>
                    <div>
                        <label for="expiry_date">Expiry Date:</label>
                        <input type="text" id="expiry_date" name="expiry_date" required>
                    </div>
                    <div>
                        <label for="cvv">CVV:</label>
                        <input type="text" id="cvv" name="cvv" required>
                    </div>
                    <div>
                        <label for="total_amount">Total Amount:</label>
                        <input type="text" id="total_amount" name="total_amount" required>
                    </div>
                    <div>
                        <input type="submit" value="Pay Now">
                    </div>
                </form>
    </div>
</section>
