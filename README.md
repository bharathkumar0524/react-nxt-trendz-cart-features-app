In this project, let's build a **Nxt Trendz - Cart Features** by applying the concepts we have learned till now.

### Refer to the image below:

<br/>

<div style="text-align: center;">
  <video style="max-width:70%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12);outline:none;" loop="true" autoplay="autoplay" controls="controls" muted>
    <source src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-output.mp4" type="video/mp4">
  </video>
</div>

### Design Files

<details>
<summary>Click to view</summary>

- [Extra Small (Size < 576px) and Small (Size >= 576px)](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-sm-output.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px)](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-lg-output.png)

</details>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>
<summary>Functionality to be added</summary>
<br/>

The app must have the following functionalities

- When an _unauthenticated user_ tries to access the **Cart** route, the page should be navigated to Login Route

- Following are the features need to implemented

- Feature 1

  - When an authenticated user tries to add the same product multiple times
    - The quantity of the product should be updated accordingly, and the count of the cart items in the header should be remained same

- Feature 2

  - The total amount and number of items in the cart should be displayed in the Cart Route

- Feature 3

  - In each cart item in the cart
    - The quantity of the product should be incremented by one when the plus icon is clicked
    - The quantity of the product should be decremented by one when the minus icon is clicked
    - When the quantity of the product is one and the minus icon is clicked, then the respective product should be removed from the cart
    - Based on the quantity of the product, the product price and the Cart Summary, i.e the total cost should be updated accordingly

- Feature 4

  - When an _authenticated user_ clicked on the remove button, Cart Item should be removed from the CartList

- Feature 5

  - When an _authenticated user_ clicked on the **Remove all** button, all the Cart Items should be removed from the cart and [EmptyCartView](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-empty-cart-view.png) should be displayed

- The following are the keys used in the context object
  - `cartList` - this variable stores the cart items
  - `removeAllCartItems` - this function is used to remove all the cart items in the cart List
  - `addCartItem` - this function adds the cart item to the cart list
  - `removeCartItem` - this function removes the cart item from the cart list
  - `incrementCartItemQuantity` - this function increases the quantity of the product in the cart list
  - `decrementCartItemQuantity` - this function decreases the quantity of the product in the cart list

</details>

<details>
<summary>Components Structure</summary>

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-component-structure-breakdown.png" alt="component structure breakdown" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

</details>

<details>
<summary>Implementation Files</summary>
<br/>

Use these files to complete the implementation:

- `src/App.js`
- `src/components/Cart/index.js`
- `src/components/Cart/index.css`
- `src/components/CartItem/index.js`
- `src/components/CartItem/index.css`
- `src/components/CartSummary/index.js`
- `src/components/CartSummary/index.css`
</details>

#### Quick Tips

<details>
<summary>Click to view Quick Tips</summary>

- The `line-height` CSS property sets the height of a line box. It's commonly used to set the distance between lines of text.

  ```
  line-height: 1.5;
  ```

    <br/>
    <img src="https://assets.ccbp.in/frontend/react-js/line-height-img.png" alt="cursor pointer" style="width:90%; max-width: 600px;"/>

</details>

### Important Note

<details>
<summary>Click to view</summary>

<br/>

**The following steps are to be followed for the tests to pass**

- `BsPlusSquare`, `BsDashSquare` icons from `react-icons` should be used for **plus** and **minus** buttons in cart item.
- The Cart Item should consist of two HTML button elements with `testid` attribute values as **plus** and **minus** respectively.
- `AiFillCloseCircle` icon from react-icons should be used for **remove** button in cartItem.
- The Cart Item should consist of an HTML button element with `testid` attribute values as **remove**.
- The product image in Cart Item Route should have the alt text as **{title}** of the product.

- Prime User credentials

  ```
   username: rahul
   password: rahul@2021
  ```

- Non-Prime User credentials

  ```
   username: raja
   password: raja@2021
  ```

- find()

  - The `find()` method returns the first item's value that satisfies the provided testing function. If no item is found, it returns `undefined`.

  **Syntax**: `arr.find(Testing Function)`

</details>

### Resources

<details>
<summary>Colors</summary>

<br/>

<div style="background-color: #0b69ff; width: 150px; padding: 10px; color: white">Hex: #0b69ff</div>
<div style="background-color: #171f46; width: 150px; padding: 10px; color: white">Hex: #171f46</div>
<div style="background-color: #616e7c; width: 150px; padding: 10px; color: white">Hex: #616e7c</div>
<div style="background-color: #ffffff; width: 150px; padding: 10px; color: black">Hex: #ffffff</div>

</details>

<details>
<summary>Font-families</summary>

- Roboto

</details>

> ### _Things to Keep in Mind_
>
> - All components you implement should go in the `src/components` directory.
> - Don't change the component folder names as those are the files being imported into the tests.
> - **Do not remove the pre-filled code**
> - Want to quickly review some of the concepts you’ve been learning? Take a look at the Cheat Sheets.
