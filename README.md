from sklearn.linear_model import LinearRegression

X=[[1000,2],[1500,3],[800,2],[1200,3],[2000,4]]
y=[50,75,40,60,90]

m=LinearRegression()
m.fit(X,y)

print("Regression Model:")
print("Price =",round(m.intercept_,2),"+",round(m.coef_[0],4),"*Area +",round(m.coef_[1],2),"*Bedrooms")
print("Intercept =",round(m.intercept_,2))
print("Coefficients =",m.coef_)
