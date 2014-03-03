TKScroller
==========

TKScroller is a simple iOS app with UIScrollView + UIPagecontrol , 
TKScroller can display one or more images , Create Tutorail screen , Show Text Details + show different viewcontrollers views,Web & Local Photos mPhotos can be zoomed and panned. 
The browser can also be used to allow the user to share image to social networking sites from main detail image view.


![logo](http://i.imgur.com/MA9WWaD.png)

## Requirements ##

1) Xcode 5 and above versions.

2) ARC


## Usage ##

1) Import `TKViewController.h` 

2) Create Array of Images and alloc TKViewController 

      NSMutableArray *images = [NSMutableArray array];
    [images addObject:[UIImage imageNamed:@"01.png"]];
    [images addObject:[UIImage imageNamed:@"02.png"]];
    TKViewController *galleryCtrl=[[TKViewController alloc]initWithImages:images];
    [self.navigationController pushViewController:galleryCtrl animated:YES];

OR use NSUrls Object 

    NSMutableArray *images = [NSMutableArray array];
    [images addObject:[NSURL URLWithString:@"http://i.imgur.com/NJTm5MI.jpg"]];
    [images addObject:[NSURL URLWithString:@"http://i.imgur.com/LVNLuNe.jpg"]];
    [images addObject:[NSURL URLWithString:@"http://i.imgur.com/SEZYqn7.jpg"]];
     
    TKViewController *galleryCtrl=[[TKViewController alloc]initWithUrls:images];
    [self.navigationController pushViewController:galleryCtrl animated:YES];




License
-------

TKGallery is available under the MIT license. See the LICENSE file for more info.
