# Basic-javascript-code
Write a JavaScript program that modifies an image by putting three vertical stripes on it - a red stripe on the left one third, a green stripe in the middle, and a blue stripe on the right one third
var img = new SimpleImage("usain.jpg");
print(img);
print(img.getWidth());
print(img.getPixel(0,0));

for( var pixel of img.values())
{
    if( pixel.getX() <= img.getWidth()/3)
    {
        pixel.setRed(255);
        
    }
    else if (pixel.getX() >= img.getWidth()/3 && pixel.getX() <= img.getWidth()*(2/3))
    {
        pixel.setGreen(255);
        
    }
    else 
    {
        pixel.setBlue(255);
    }
    
        
}
    print(img);
