### **Day 5: Working with the Django Admin Interface**

1. **Registering the Model in the Admin Panel:**
   - To access and manage your model via the Django admin interface, register it in the `admin.py` file in your app.
   
Example of registering the model in `admin.py`:

   ```python
   from django.contrib import admin
   from .models import MyModel

   admin.site.register(MyModel)
   ```

2. **Accessing the Django Admin Panel:**
   - Start the development server (`python manage.py runserver`) and go to `http://127.0.0.1:8000/admin/`.
   - Log in using the superuser account created during the initial setup.
   - You should see your `MyModel` listed. You can add, edit, and delete instances of the model using the admin interface.

### **Practice Tasks:**
- Experiment with different field types (CharField, IntegerField, ForeignKey, etc.) in the model.
- Create relationships between different models (One-to-One, One-to-Many, Many-to-Many) and explore how they're represented in the admin interface.
