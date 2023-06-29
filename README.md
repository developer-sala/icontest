# TravelUs 🚌
🔗[TravelUs 바로가기](https://travels-us.netlify.app/ )
- ID: travelus_official@travelus.com
- PW: 123123

### 목차


### 4번 리뷰<br> 
페이지 링크 - https://github.com/FRONTENDSCHOOL5/final-04-fearless4/blob/main/src/pages/userProfile/ProductsForSale.jsx<br>

✅ 범위: 
- ProductsForSale.jsx파일 115 ~ 217 line

✅ 전체 개요 :
- 요건에 맞는 상품을 정렬하여 보여주는 기능입니다.

✅ 기능 내용
- 사용자들이 함께 떠나는 상품 목록에서 🔥추천 상품이나 🤑할인 상품 버튼을 클릭하면, 해당 요건에 맞는 상품이 정렬되어 보여집니다.
- 상품 판매자가 상품 등록할 때 제목 앞에 [추천], [할인] 문구를 넣어주면 해당 기능이 적용됩니다.
- 사용자들이 추천이나 할인 상품을 보다가 전체 상품을 보고 싶을 때, # 전체 상품 버튼을 누르면 처음처럼 전체 상품 목록을 볼 수 있습니다.
```jsx
useEffect(() => {
		if (resProd.length !== 0) {
			const product = resProd.map((item) => (
				<ProductList
					key={item.id}
					onClick={() => {
						handleModalOpen(item);
					}}
				>
					<ProductImg
						src={item.itemImage}
						alt={`${item.itemName}의 상품 이미지`}
					/>
					<ProductName>{item.itemName}</ProductName>
					<ProductPrice>{item.price.toLocaleString()}원</ProductPrice>
				</ProductList>
			));
			setProductData(product);
		}
	}, [resProd]);

	const handleShowAllProducts = () => {
		const products = resProd.map((item) => (
			<ProductList
				key={item.id}
				onClick={() => {
					handleModalOpen(item);
				}}
			>
				<ProductImg
					src={item.itemImage}
					alt={`${item.itemName}의 상품 이미지`}
				/>
				<ProductName>{item.itemName}</ProductName>
				<ProductPrice>{item.price.toLocaleString()}원</ProductPrice>
			</ProductList>
		));
		setProductData(products);
	};

	const handleShowRecommendedItems = () => {
		const recommendedProducts = resProd.filter((item) =>
			item.itemName.includes('[추천]')
		);
		const products = recommendedProducts.map((item) => (
			<ProductList
				key={item.id}
				onClick={() => {
					handleModalOpen(item);
				}}
			>
				<ProductImg
					src={item.itemImage}
					alt={`${item.itemName}의 상품 이미지`}
				/>
				<ProductName>{item.itemName}</ProductName>
				<ProductPrice>{item.price.toLocaleString()}원</ProductPrice>
			</ProductList>
		));
		setProductData(products);
	};

	const handleShowDiscountedItems = () => {
		const discountedProducts = resProd.filter((item) =>
			item.itemName.includes('[할인]')
		);
		const products = discountedProducts.map((item) => (
			<ProductList
				key={item.id}
				onClick={() => {
					handleModalOpen(item);
				}}
			>
				<ProductImg
					src={item.itemImage}
					alt={`${item.itemName}의 상품 이미지`}
				/>
				<ProductName>{item.itemName}</ProductName>
				<ProductPrice>{item.price.toLocaleString()}원</ProductPrice>
			</ProductList>
		));
		setProductData(products);
	};

	return (
		<>
			{resProd.length === 0 ? null : (
				<WrapAll>
					<Title>함께 떠나는 상품</Title>
					<SortedButton first onClick={handleShowAllProducts}>
						# 전체 상품
					</SortedButton>
					<SortedButton onClick={handleShowRecommendedItems}>
						🔥추천 상품
					</SortedButton>
					<SortedButton onClick={handleShowDiscountedItems}>
						🤑할인 상품
					</SortedButton>
					<Scroll>
						<ProductsContainer>{productData}</ProductsContainer>
					</Scroll>
				</WrapAll>
			)}

```

🤔 코드 리뷰에서 궁금한 점: 
- 전체 상품, 추천 상품, 할인 상품 버튼을 선택에서 화면에 보여주는 코드가 다 중복이 되는데요, 혹시 중복된 코드를 줄이거나 코드를 개선할 수 있는 방법이 있을까요?



### 4번 리뷰<br> 
페이지 링크 -<br> 
상품 등록(https://github.com/FRONTENDSCHOOL5/final-04-fearless4/blob/main/src/pages/userProfile/MyProfile.jsx) → 버튼 누르면 이동하는 상품등록 페이지(https://github.com/FRONTENDSCHOOL5/final-04-fearless4/blob/main/src/pages/product/Product.jsx)<br><br>
상품 수정(https://github.com/FRONTENDSCHOOL5/final-04-fearless4/blob/main/src/pages/userProfile/ProductsForSale.jsx) → 버튼 누르면 이동하는 상품수정 페이지(https://github.com/FRONTENDSCHOOL5/final-04-fearless4/blob/main/src/pages/userProfile/ProductsForSaleEdit.jsx)

✅ 범위: 
- MyProfile.jsx 파일 195 line 상품등록 버튼 → ProductsForSale.jsx파일 이동
- ProductsForSale.jsx 파일 226 line 수정 버튼 → ProductsForSaleEdit.jsx파일 이동

✅ 전체 개요 :
- 상품등록 또는 수정 버튼을 누르면 상품등록/상품수정 페이지로 이동합니다.

✅ 기능 내용
- tkdvna 상품록: 상품명, 가격, 판매링크 모두 입력하면 mMyProfile 페이지에 상품이 등록됩니다.
- mMyProfile 페이지 상품 수정ㅇ ㅏㅍ판매 상품을 입력하고 서정버튼을 누르면 수정할 수 있습니다. 
  

🤔 코드 리뷰에서 궁금한 점: 
- MyProfile.jsx 파일 195 line 상품등록 버튼 → ProductsForSale.jsx파일 이동하여 상품 등록을 할 수 있고, ProductsForSale.jsx 파일 226 line 수정 버튼 → ProductsForSaleEdit.jsx파일 이동하면 상품 수정을 할 수 있는데 상품 등록페이지와 상품 수정 페이지가 사실상 형식은 똑같습니다. 단지 수정페이지는 기존 등록되어 있는 정보를 가져오는 것만 다릅니다. 중복된 페이지라고 생각이 드는데 두 페이지를 합치거나 더 효율적인 방법이 없을까요? 

