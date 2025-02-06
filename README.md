# Craft CMS Setup Guide  

## Introduction  
Welcome! This guide outlines the standard process for setting up new websites using Craft CMS. While we have a general structure in place, this document will help define specifics to ensure consistency and efficiency across all projects.  

As our team scales and the demand for new sites grows, having a standardized setup will allow us to work more efficiently while maintaining high-quality builds. This guide will evolve over time as we refine our approach, so feel free to contribute updates or suggestions.  
 
## Prerequisites  
Before setting up Craft CMS, ensure you have the following installed:  
- PHP (version 8.0 or higher)  
- Composer  
- MySQL or PostgreSQL database  
- DDEV

## Avoid
- Redactor (plug-in, app has been abandoned)
- XAMPP, Apache (craft prefers ddev)

# Installation Steps For Existing Repo  

### 1. Clone the Project Repository  
```sh
git clone https://github.com/yourusername/your-craft-project.git

cd your-craft-project
```
### 2. Set Up .env
```sh
cp .env.example .env
```

### 3. Update database credentials
```sh
DB_DATABASE=your_database_name  
DB_USER=your_database_user  
DB_PASSWORD=your_database_password  
```
### 4. Set File Permissions
```sh
chmod -R 775 storage/ config/ web/cpresources/
```

### 5. Run craft setup
```sh
php craft setup
```

### . 6
```sh

```

# From Scratch

### . 1
```sh
mkdir new
```

### . 2
```sh
ddev config --project-type=craftcms --docroot=web
```

### . 3
```sh
ddev composer create -y --no-scripts craftcms/craft
```

### . 4
```sh
ddev launch
```


### . S
```sh

```
