# Project Responsive Web Design using Bootstrap
# Date:17-12-2024
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
website.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech News</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        #home {
            background: url('banner.png') no-repeat center center/cover;
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
        }
        #latest .news-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 20px;
            border-bottom: 1px solid #ddd;
            padding-bottom: 15px;
        }
        #latest .news-item img {
            width: 120px;
            height: 80px;
            object-fit: cover;
            margin-right: 15px;
        }
        #latest .news-item h5 {
            margin: 0 0 5px;
            font-size: 1.1rem;
        }
        #latest .news-item p {
            margin: 0;
            font-size: 0.9rem;
            color: #555;
        }
    </style>
</head>
<body>

<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
        <a class="navbar-brand" href="#">TechNews</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ms-auto">
                <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="#home">Home</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#latest">Latest News</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#reviews">Reviews</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#contact">Contact</a>
                </li>
            </ul>
        </div>
    </div>
</nav>

<section id="home" class="bg-primary text-white text-center py-5">
    <div class="container">
        <h1>Welcome to TechNews</h1>
        <p class="lead">Stay updated with the latest in technology and gadgets.</p>
        <a href="#latest" class="btn btn-light mt-3">Explore News</a>
    </div>
</section>

<section id="latest" class="py-5">
    <div class="container">
        <h2 class="text-center">Latest News</h2>
        <div class="mt-4">
            <div class="news-item">
                <img src="news1.png" alt="News Image">
                <div>
                    <h5>Mobile</h5>
                    <p>	
                        Redmi Turbo 4 to Get MediaTek Dimensity 8400-Ultra SoC; Realme Neo 7 SE With Dimensity 8400 Teased</p>
                </div>
            </div>
            <div class="news-item">
                <img src="news2.png" alt="News Image">
                <div>
                    <h5>Telecom</h5>
                    <p>	
                        Airtel Wi-Fi Plans Starting From Rs. 699 Now Bundles Free Zee5 OTT Subscription</p>
                </div>
            </div>
            <div class="news-item">
                <img src="news3.png" alt="News Image">
                <div>
                    <h5>Tablets</h5>
                    <p>	
                        iPad 11 to Reportedly Be Launched Early Next Year, Could Arrive With iPadOS 18.3</p>
                </div>
            </div>
            <div class="news-item">
                <img src="news4.png" alt="News Image">
                <div>
                    <h5>AI</h5>
                    <p>	
                        South Korean Researchers Unveil Wearable ‘Iron Man’ Exoskeleton Robot to Help People with Paraplegia Walk</p>
                </div>
            </div>
            <div class="news-item">
                <img src="news5.png" alt="News Image">
                <div>
                    <h5>Mobiles</h5>
                    <p>	
                        Realme 14 Pro 5G Series With 1.5K Display and 6,000mAh Battery Teased in Suede Grey Colour Ahead of India Launch</p>
                </div>
            </div>
        </div>
    </div>
</section>

<section id="reviews" class="bg-light py-5">
    <div class="container">
        <h2 class="text-center">Tech Reviews</h2>
        <div class="row mt-4">
            <div class="col-md-6">
                <h5>Gadget Review: Vivo X200 Pro</h5>
                <p>Vivo X200 Pro is already one of the contenders for the best smartphone camera of 2025</p>
            </div>
            <div class="col-md-6">
                <h5>Mobile Launch: IQOO 13</h5>
                <p>iQOO, a sub-brand of Vivo, is known for making phones that are performance-focused and value for money. After the success of the iQOO 12 from last year</p>
            </div>
        </div>
    </div>
</section>

<section id="contact" class="py-5">
    <div class="container">
        <h2 class="text-center">Contact Us</h2>
        <form class="mt-4">
            <div class="mb-3">
                <label for="name" class="form-label">Name</label>
                <input type="text" class="form-control" id="name" placeholder="Enter your name">
            </div>
            <div class="mb-3">
                <label for="email" class="form-label">Email</label>
                <input type="email" class="form-control" id="email" placeholder="Enter your email">
            </div>
            <div class="mb-3">
                <label for="message" class="form-label">Message</label>
                <textarea class="form-control" id="message" rows="4" placeholder="Your message"></textarea>
            </div>
            <button type="submit" class="btn btn-primary">Send Message</button>
        </form>
    </div>
</section>

<footer class="bg-dark text-white text-center py-3">
    <p>&copy; 2024 TechNews. All Rights Reserved.</p>
</footer>

</body>
</html>

~~~
# OUTPUT:
![projectweb](https://github.com/user-attachments/assets/00a9d3b1-e9d4-40b2-895d-f7a4cde5d550)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
