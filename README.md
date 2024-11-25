# CSS GRID

This project demonstrates a responsive CSS Grid Layout for displaying "Student Profiles." The grid is designed to adjust dynamically to various screen sizes, ensuring a visually appealing and user-friendly experience.

## Features
1. Responsive Design:
- Automatically adjusts the number of columns based on the available screen width.
- Uses auto-fit and minmax properties to ensure flexibility.

2. Stylish Cards:
- Each student profile card is styled with rounded corners, padding, and shadow effects.
- Hover and active states add interactivity to the cards.

3. Centered Layout:
- The grid is centered and constrained with a max-width for a clean and balanced appearance.

## Code Overview
### Grid Container

```html
<section class="student-profiles">
    <div class="student-profile">Student 1</div>
    <div class="student-profile">Student 2</div>
    <div class="student-profile">Student 3</div>
</section>
```
## CSS Grid Imlementation
### Grid Container
```html
.student-profiles {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    padding: 20px;
    max-width: 1200px;
    margin: 0 auto;
}
```
- display: grid;: Enables grid layout.
- grid-template-columns:
- repeat(auto-fit, minmax(200px, 1fr)): Creates flexible columns where each is at least 200px wide and can grow to fill available space.
- gap: Adds spacing between grid items.
- max-width: Limits the grid's overall width for better aesthetics.
- margin: 0 auto;: Centers the grid on the page.

### Grid Items (Cards)
```html
.student-profile {
    background-color: #ffffff;
    border: 1px solid #ddd;
    border-radius: 10px;
    padding: 16px;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

.student-profile:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 10px rgba(0, 0, 0, 0.15);
}

.student-profile:active {
    transform: translateY(0);
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
```
- Card Styling
-  border-radius: Creates rounded corners.
- box-shadow: Adds depth to the card.
- transition: Smooth animation for hover and active states.

## Output

![{7FE002EF-A7CB-4D8D-9CD0-31D5357CD888}](https://github.com/user-attachments/assets/dea9fd66-2934-4eab-840d-701c233ccc58)

![{147D1436-C6AA-468F-A92E-4F1C05F0DD91}](https://github.com/user-attachments/assets/50791df6-2d3b-48fe-9242-a612391ec3b2)

![{738A5AA2-BF4E-45D4-B376-CF40BB7A8FD7}](https://github.com/user-attachments/assets/03990d52-3152-456a-ae53-3428140a4a8d)




