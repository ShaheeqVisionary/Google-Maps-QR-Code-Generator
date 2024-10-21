
# Google Maps QR Code Generator

This Python script allows you to generate a QR code for any Google Maps link. You can use the QR code to easily share locations through printed media, social media, or just scanning the code from your phone.

## Table of Contents

- [Requirements](#requirements)
- [How to Use](#how-to-use)
- [Customization](#customization)
- [Example QR Code](#example-qr-code)
- [License](#license)

## Requirements

To run this script, you need Python installed on your machine along with the following libraries:

- `qrcode`: For generating the QR code.
- `Pillow`: Used for saving the QR code image in PNG format.

You can install these dependencies using pip:

```bash
pip install qrcode[pil]
```

## How to Use

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/qr-code-generator.git
   ```
   
2. Navigate to the project directory:
   ```bash
   cd qr-code-generator
   ```

3. Open the `qr_code_generator.py` file in any text editor and replace the `url` variable with your Google Maps link (or any other link):

   ```python
   url = "https://goo.gl/maps/WRoCoZdn3AQ6Ads46"
   ```

4. Run the Python script to generate the QR code:

   ```bash
   python qr_code_generator.py
   ```

5. The QR code image will be saved as `google_maps_qr_code.png` in the current directory.

## Customization

You can customize the following aspects of the QR code:

- **Size**: Adjust the `box_size` parameter in the script to change the size of each QR code box.
- **Error Correction**: The `error_correction` parameter controls how much damage the QR code can tolerate. Available levels are:
  - `ERROR_CORRECT_L`: Up to 7% damage.
  - `ERROR_CORRECT_M`: Up to 15% damage.
  - `ERROR_CORRECT_Q`: Up to 25% damage.
  - `ERROR_CORRECT_H`: Up to 30% damage.
- **Colors**: You can change the colors of the QR code by modifying the `fill` and `back_color` parameters.

## Example QR Code

After running the script, a QR code image like this will be generated:

![QR Code Example](google_maps_qr_code.png)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

