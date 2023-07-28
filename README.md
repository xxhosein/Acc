from flask import Flask

# ایجاد یک نمونه از کلاس Flask با نام app
app = Flask(__name__)

# تعریف مسیر اصلی و ویو آن
@app.route('/')
def hello():
    return "Hello, World!"

# تابع اصلی برای اجرای برنامه
if __name__ == '__main__':
    # اجرای برنامه با پارامتر‌های مشخص
    app.run(debug=True)
