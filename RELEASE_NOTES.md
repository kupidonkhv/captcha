# Release Notes: v3.5.0 - Laravel 12 Support

## 🎉 Release Overview
Version 3.5.0 brings full compatibility with Laravel 12 while maintaining backward compatibility with Laravel 5-11.

## ✅ What's New

### Full Laravel 12 Compatibility
- **Tested with Laravel 12.29.0**
- **All Illuminate components updated to v12.29.0**
- **Verified compatibility with PHP 8.2.29 and 8.3**

### Updated Dependencies
- **Intervention Image**: ^3.7 (tested with 3.11.4)
- **PHP**: 7.2 - 8.3 support
- **Laravel**: 5.x - 12.x support

### 🧪 Comprehensive Testing
The package has been thoroughly tested in a Laravel 12 environment:

#### Core Functionality Tests
- ✅ Image generation and rendering
- ✅ Cache integration (Cache::pull() method compatibility)
- ✅ Session handling (Session::remove() method compatibility)
- ✅ Validation methods and rules
- ✅ All configuration presets (default, flat, mini, inverse)

#### Integration Tests
- ✅ Intervention Image methods compatibility
- ✅ GD extension functionality
- ✅ Multiple character sets and fonts
- ✅ Different image quality settings

### 📦 Installation
```bash
composer require kupidonkhv/captcha
```

### 🔧 Configuration
Publish configuration file:
```bash
php artisan vendor:publish --provider="Mews\Captcha\CaptchaServiceProvider"
```

### 🚀 Usage Examples
```php
// In your form
{!! captcha_img() !!}

// Validation
'captcha' => 'required|captcha'

// Using facade
Captcha::create();
```

### 📋 System Requirements
- **PHP**: 7.2 - 8.3
- **Laravel**: 5.x - 12.x
- **Extensions**: GD, FileInfo, MBString
- **Intervention Image**: ^3.7

### 🐛 Bug Fixes & Improvements
- Updated package name from mews/captcha to kupidonkhv/captcha
- Fixed documentation links and badges
- Improved README with Laravel 12 specific instructions
- Verified all deprecated method replacements

### 🔗 Links
- **GitHub Repository**: https://github.com/kupidonkhv/captcha
- **Packagist**: https://packagist.org/packages/kupidonkhv/captcha
- **Release**: https://github.com/kupidonkhv/captcha/releases/tag/v3.5.0

### 🙏 Credits
Forked from mews/captcha with continued maintenance and Laravel 12+ support.

---
*Release Date: September 16, 2025*
*Version: 3.5.0*
