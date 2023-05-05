### Hi there 👋
foreach ($results as $row) {
    $unit_cost = $row['unit_cost'];
    $unit_price = $row['unit_price'];
    $name = $row['name'];
    $product_id = $row['product_id'];
    $desired_quantity = $row['desired_quantity'];
    
    // Check if unit cost matches unit price, with tolerance of 0.01
    if (abs($unit_cost - $unit_price) > 0.01) {
      $diff_percentage = abs($unit_cost - $unit_price) / $unit_price * 100;
      flash("Warning: The unit cost of {$name} (product ID: {$product_id}) in your cart differs from its unit price by {$diff_percentage}%");
    }
<!--
**mateamilloshi/mateamilloshi** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
