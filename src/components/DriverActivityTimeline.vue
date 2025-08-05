<template>
  <div class="card mb-3">
    <div class="card-body">
      <h5 class="card-title fw-bold mb-4">Driver Activity Timeline</h5>
      <ul class="timeline list-unstyled">
        <li class="timeline-item">
          <div class="timeline-marker bg-success"></div>
          <div class="timeline-content">
            <strong>Started working</strong> at Treffix.id

            <div class="small text-muted">08:15 AM</div>
          </div>
        </li>

        <li class="timeline-item">
          <div class="timeline-marker bg-primary"></div>
          <div class="timeline-content">
            <strong>Driving to client location</strong>
            <div class="small text-muted">09:30 AM</div>
          </div>
        </li>

        <li class="timeline-item">
          <div class="timeline-marker bg-warning"></div>
          <div class="timeline-content">
            <strong>Stopped for a coffee break</strong> at Kopi Kenangan
            <div class="small text-muted">11:00 AM</div>
          </div>
        </li>

        <li class="timeline-item">
          <div class="timeline-marker bg-info"></div>
          <div class="timeline-content">
            <strong>Arrived at meeting</strong> with client
            <div class="small text-muted">12:00 PM</div>
          </div>
        </li>

        <li class="timeline-item">
          <div class="timeline-marker bg-dark"></div>
          <div class="timeline-content">
            <strong>Back home</strong> and rest
            <div class="small text-muted">06:30 PM</div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.timeline {
  position: relative;
  padding-left: 20px;
  border-left: 3px solid #dee2e6;
}

.timeline-item {
  position: relative;
  margin-bottom: 1.5rem;
}

.timeline-marker {
  width: 14px;
  height: 14px;
  border-radius: 50%;
  position: absolute;
  left: -8px;
  top: 4px;
  border: 2px solid #fff;
  box-shadow: 0 0 0 3px #dee2e6;
}

.timeline-content {
  margin-left: 1rem;
}
</style>
