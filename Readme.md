# Hướng dẫn triển khai Backend

## **1. Cài đặt Backend**

### **Clone và build các repository**

```bash
# Clone và build service crawler
git clone https://github.com/nguoibattrang/crawler.git
cd crawler
docker build -t nbt_crawler .

# Clone và build service forwarder
git clone https://github.com/nguoibattrang/forwarder.git
cd forwarder
docker build -t nbt_forwarder .
```

---

### **Tạo các thư mục cần thiết**

```bash
sudo mkdir -p /opt/nbt/crawler
sudo mkdir -p /opt/nbt/forwarder
sudo mkdir -p /opt/nbt/kafka
```

> **Tham khảo nội dung các thư mục tại**:  
> [https://github.com/nguoibattrang/installer/tree/main/](https://github.com/nguoibattrang/installer/tree/main/)

---

### **Cập nhật cấu hình**
- Cập nhật cấu hình cho từng service trong các thư mục tương ứng.  
- Start các Docker container trong từng thư mục.

---

## **2. Kết quả triển khai**

### **Dữ liệu crawl được đẩy vào Kafka**

![Dữ liệu crawl Kafka](https://github.com/user-attachments/assets/cb798c75-edd7-4d39-bf85-f7a4c3df482c)

---

### **Dữ liệu đẩy thành công tới Dify**

![Dữ liệu tới Dify](https://github.com/user-attachments/assets/c5c3ff7c-2f7e-4455-925b-11a106231453)

### **Dữ liệu trong Dify**
![Dữ liệu trong Dify](https://github.com/user-attachments/assets/c935d637-8a41-4adb-b041-a9a489c7aaa8)
![Cấu hình Dify](https://github.com/user-attachments/assets/517ab737-e4e7-4646-980d-c7b16f025a5a)

