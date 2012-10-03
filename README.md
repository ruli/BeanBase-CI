# BeanBase-CI

BeanBase and CodeIgniter Integration

> Notice: This project is based on CI 2.1.2 and RedBean 3.2, backward compatibility is not guaranteed (you're welcome to make compatibility patches). RBB and BaseModel (MY_Model) are tested under PHP 5.3/5.4 environment, for that, backward compatibility is not going to happen (a tiny effort to push PHP forward faster).

Core project Details, Manual, Docs & More at [BeanBase GitHub Page](http://ruli.github.com/BeanBase)

## Installation
1. Copy `application/libraries/Rb.php` into your `application/libraries` directory
2. Copy `application/third_party/rbb.php` into your `application/third_party` directory
3. Grab RedBean (the single rb.php file) from the [official site](http://redbeanphp.com/), and place that in your `application/third_party` directory
4. In your controllers and/or models, where appropriate (usually constructors), load the Rb library by using `$this->load->library('rb')`
5. __Optional:__ If you wish to use `BaseModel`
    a. Copy `application/core/MY_Model.php` into your `application/core` directory
    b. In your models, instead of extending `CI_Model`, extend `MY_Model` now

> Notice: If you wish to take a more graduate approach of adopting RBB and/or BaseModel, simply do all of above, and start with new(er) models/controllers to test out what BeanBase and RedBean have to offer. Once you start liking them, you can consider rewrite DB interaction logics model by model (and/or controller by controller).

> Notice: To learn how to use BeanBase, check out the core project page at [BeanBase GitHub Page](http://ruli.github.com/BeanBase). BeanBase-CI specific examples will follow up (eventually).