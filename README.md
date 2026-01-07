🗂️ Accordion with Icons

A premium, interactive accordion component built with Tailwind CSS and Lucide Icons. This component features a sophisticated color palette, smooth transitions, and a clear information hierarchy, making it ideal for FAQs, feature lists, or instructional content.

🚀 Live Demo

Explore the Accordion Component Here

✨ Project Overview

The Accordion with Icons is designed to present large amounts of information in a compact, organized manner. It prioritizes visual clarity through the use of distinct brand-aligned icons and smooth height animations.

Key Features

Interactive Icon States: Icons reside in containers that shift from a subtle aqua to a vibrant teal when active, providing clear visual feedback.

Smooth Animations: Uses custom CSS cubic-bezier transitions for a professional "slide-down" effect and rotating chevrons.

Modern Typography: Built with the 'Inter' font family, featuring strict uppercase tracking for subheadings and balanced line heights for body text.

Custom Scrollbar: Enhanced UI experience with brand-styled scrollbars that match the Midnight Blue and Teal aesthetic.

Single-Active Logic: The JavaScript toggle ensures only one section is open at a time, reducing cognitive load for the user.

🛠️ Technical Implementation

Styling Engine: Tailwind CSS for layout utility and a custom <style> block for complex CSS transitions (max-height and opacity).

Iconography: Integration of the Lucide Icon Library via CDN, allowing for lightweight and scalable vector graphics.

Responsive Design: Fully responsive container that adjusts padding and font sizes between mobile and desktop views.

Visual Design Tokens:

Midnight Blue (#1f2a52): Header and primary text.

Teal (#00bec7): Active accents and subheading tracking.

Light Aqua (#d2f0f0): Inactive icon backgrounds and scrollbar tracks.

Slate Grey (#abb5bf): Secondary text and UI borders.

📂 Structure and Usage

The component is entirely self-contained within a single HTML file, making it easy to drop into existing projects.

Header: Introduces the content category with a stylized background and decorative blur accents.

Accordion Items: Each item is a div containing a toggle button and a content panel.

JavaScript Logic: The toggleAccordion function manages the active class across the DOM.

function toggleAccordion(element) {
    const allItems = document.querySelectorAll('.accordion-item');
    const isActive = element.classList.contains('active');

    // Close all items to maintain single-open focus
    allItems.forEach(item => item.classList.remove('active'));

    // If the clicked item wasn't active, open it
    if (!isActive) {
        element.classList.add('active');
    }
}


📄 License

MIT License - Developed as part of the accounts-eles UI component library.
