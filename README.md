# PrettyQr

## Overview

pretty_qr is a library based on [rQrCode] (http://github.com/whomwah/rqrcode) built to make beautiful QR codes. 

What it can do for now : 
* QR codes are rendered with rounded corners
* You can specify colors : foreground, background, marking corners. 

## Resources
* QR code is a registered trademark by [Denso Wave inc] (http://www.qrcode.com/en/)
* This gem is based on [rQRCode] (http://github.com/whomwah/rqrcode)
* THis work is inspired by [liquidcode] (http://github.com/jooray/liquidcode)

## Installation

Add this line to your application's Gemfile:

    gem 'pretty_qr'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install pretty_qr

## Basic Usage

    qr_code = PrettyQr::QrCode.new('http://google.com', { block_size: 10, foreground_color: 'purple' })
    qr_code.render_to_file 'examples/images/basic.png'
    
It gives you a file like 

![Basic image](https://raw2.github.com/benoitma/pretty_qr/master/examples/images/basic.png)

## Custom corners

Use the option : ```corners_color``` to make a different color in the corners. 
    
It gives you a qr_code a bit more beautiful

![Basic image](https://raw2.github.com/benoitma/pretty_qr/master/examples/images/custom_corners.png)

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
