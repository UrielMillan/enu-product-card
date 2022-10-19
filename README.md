#Ejemplo

```
import {ProductCard, ProductImage, ProductTitle, ProductButtons } from 'enu-product.card'
```

```
<ProductCard
  product={product}
  onChange={onProductCountChange}
  value={shoppingCart[product.id]?.count || 0}
  initialValues={{
      count: 4,
      maxCount: 10
  }}
>

  {
    ({reset, isMaxCountReached, increaseBy, count}) => (
      <>
        <ProductImage  />
        <ProductTitle  />
        <ProductButtons />
      </>
    )
  }
</ProductCard>
```