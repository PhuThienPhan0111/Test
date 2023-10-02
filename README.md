# Test
 document.getElementById('root')
Scaffold-DbContext "Server=DESKTOP-P388UUP\SQLEXPRESS; DataBase=TEST_REACT; Integrated Security=True;TrustServerCertificate=True" Microsoft.EntityFrameworkCore.SqlServer -OutPutDir Models

FE (web có thể dùng reactjs / javascript / vuejs.., ưu tiên reactjs): cho phép người dùng nhập vào danh sách Customer (Full Name, Date of Birth - DOB, Email), Shop (Name, Location) và Product (Name, Price). Một Customer có thể mua nhiều Product ở nhiều Shop. Một Shop có nhiều Product. Cần nhập ít nhất là 30 Customer, 3 Shop, và 30 Product. Cho phép tìm kiếm Product trong khoảng Price.
BE (.netcore, entity fw core): lưu trữ Customer/Shop/Product vào database. Load dữ liệu từ database và tiến hành sắp xếp theo qui luật: Customer.Email theo thứ tự alphabet tăng dần, Shop.Location theo thứ tự alphabet giảm dần, Product.Price theo thứ tự giảm dần => Kết quả sắp xếp sẽ được trả về FE để hiện thị lên UI (Nếu không đủ 30 Customer, 3 Shop, và 30 Product, UI sẽ hiển thị thông báo lỗi Không Đủ Dữ Liệu).
 
--> FE OUTPUT:

Table Headers
------------------------------------------------------------------------
 Customer (Name - Email) : Shop (Name - Location): Product (Name - Price)
  Customer (Name - Email) : Shop (Name - Location): Product (Name - Price)
  ...                  
  Customer (Name - Email) : Shop (Name - Location): Product (Name - Price)
  ********           
  Customer (Name - Email) : Shop (Name - Location): Product (Name - Price)
  Customer (Name - Email) : Shop (Name - Location): Product (Name - Price)
  ...                  
  Customer (Name - Email) : Shop (Name - Location): Product (Name - Price)
  ********
 
==> làm video ngắn demo cho code flow và chạy tính năng trên UI
