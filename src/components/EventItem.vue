<template>
  <div class="events-container">
    <h2>Events</h2>
    <div class="event-card">
      <div class="event-image">
        <img src="@/assets/gal3.webp" alt="FDA Philippines poster compitition">
      </div>
      <div class="event-info">
        <h3>FDA Philippines</h3>
        <p>Join the FDA Philippines Poster Competition, a creative endeavor focused on designing impactful visual solutions for regulatory challenges in public health and safety.</p>
      </div>
    </div>
    <div class="event-card">
      <div class="event-image">
        <img src="@/assets/gal2.webp" alt="Davao Region Poster Competition">
      </div>
      <div class="event-info">
        <h3>PDavao Regional</h3>
        <p>Engage in the Davao Region Poster Competition, a platform for showcasing artistic talent and addressing local issues through compelling visual communication.</p>
      </div>
    </div>
    <div class="event-card">
      <div class="event-image">
        <img src="@/assets/gal8.webp" alt="Esports Tournament">
      </div>
      <div class="event-info">
        <h3>Esports Tournament (PSITS)</h3>
        <p>A competitive gaming event featuring various esports titles.</p>
      </div>
    </div>
  </div>
</template>

<style>
.events-container {
  text-align: center;
  margin-top: 50px;
}

.events-container h2 {
  margin-bottom: 30px;
}

.event-card {
  display: flex;
  flex-direction: row; 
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
  max-width: 600px; 
  margin: 0 auto; 
}

.event-card:hover {
  transform: translateY(-5px);
}

.event-image {
  width: 40%; 
  overflow: hidden;
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
}

.event-image img {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.event-info {
  width: 60%; 
  padding: 20px;
  background-color: #000000; 
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
}

.event-info h3 {
  margin-top: 0;
}

.event-info p {
  margin-bottom: 0;
}


</style>