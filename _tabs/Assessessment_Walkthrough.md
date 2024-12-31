---
title: Your SNWG Assessment Journey
author: SNWG MO
date: 2024-12-30 12:00:00 +0600
categories: [Guide]
tags: [overview, getting-started]
order: 4
---

<!-- Custom styles - add to assets/css/style.scss -->
<style>
:root {
    --primary: #3b82f6;
    --primary-light: rgba(59, 130, 246, 0.1);
    --success: #10b981;
    --warning: #f59e0b;
}

.hero-section {
    background: linear-gradient(135deg, var(--primary), #60a5fa);
    color: white;
    padding: 3rem 2rem;
    border-radius: 1rem;
    margin: -1rem -1.5rem 2rem -1.5rem;
    text-align: center;
    position: relative;
    overflow: hidden;
}

.hero-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: url('data:image/svg+xml,<svg width="20" height="20" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><rect width="1" height="1" fill="rgba(255,255,255,0.1)"/></svg>') repeat;
    opacity: 0.2;
}

.hero-section h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    color: white;
}

.timeline {
    position: relative;
    margin: 3rem 0;
    padding: 2rem 0;
}

.timeline-line {
    position: absolute;
    top: 50%;
    left: 0;
    right: 0;
    height: 4px;
    background: var(--primary-light);
    transform: translateY(-50%);
}

.phase-wrapper {
    display: flex;
    justify-content: space-between;
    position: relative;
    z-index: 1;
}

.phase {
    text-align: center;
    flex: 1;
    padding: 0 15px;
    position: relative;
}

.phase-marker {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: var(--sidebar-bg);
    border: 3px solid var(--border-color);
    margin: 0 auto 15px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    position: relative;
    transition: all 0.3s ease;
}

.phase.current .phase-marker {
    background: var(--primary);
    color: white;
    border-color: var(--primary);
    box-shadow: 0 0 0 6px var(--primary-light);
    animation: pulse 2s infinite;
}

.phase.completed .phase-marker {
    background: var(--success);
    color: white;
    border-color: var(--success);
}

.phase-content {
    opacity: 0.7;
    transition: all 0.3s ease;
}

.phase.current .phase-content {
    opacity: 1;
}

.phase:hover .phase-content {
    opacity: 1;
    transform: translateY(-5px);
}

.action-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 1.5rem;
    margin: 2rem 0;
}

.action-card {
    background: var(--card-bg);
    border-radius: 1rem;
    padding: 1.5rem;
    border: 1px solid var(--border-color);
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}

.action-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 4px;
    background: var(--primary);
    transform: scaleX(0);
    transition: transform 0.3s ease;
    transform-origin: left;
}

.action-card:hover::before {
    transform: scaleX(1);
}

.action-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.resource-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1.5rem;
    margin: 2rem 0;
}

.resource-card {
    background: var(--card-bg);
    border-radius: 1rem;
    padding: 1.5rem;
    border: 1px solid var(--border-color);
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
    cursor: pointer;
}

.resource-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.resource-icon {
    font-size: 2rem;
    margin-bottom: 1rem;
    color: var(--primary);
}

.timeline-table {
    width: 100%;
    border-collapse: separate;
    border-spacing: 0 0.5rem;
    margin: 2rem 0;
}

.timeline-table th,
.timeline-table td {
    padding: 1rem;
    background: var(--card-bg);
    border: none;
}

.timeline-table tr {
    transition: all 0.3s ease;
}

.timeline-table tr:hover {
    transform: translateX(5px);
}

.timeline-table td:first-child {
    border-radius: 0.5rem 0 0 0.5rem;
}

.timeline-table td:last-child {
    border-radius: 0 0.5rem 0.5rem 0;
}

.status-badge {
    display: inline-block;
    padding: 0.25rem 0.75rem;
    border-radius: 1rem;
    font-size: 0.875rem;
    font-weight: 500;
}

.status-badge.in-progress {
    background: var(--primary-light);
    color: var(--primary);
}

.status-badge.upcoming {
    background: rgba(249, 115, 22, 0.1);
    color: #f97316;
}

.help-container {
    background: var(--card-bg);
    border-radius: 1rem;
    padding: 2rem;
    text-align: center;
    margin: 3rem 0;
    border: 1px solid var(--border-color);
    position: relative;
}

.help-icon {
    width: 60px;
    height: 60px;
    background: var(--primary);
    color: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.5rem;
    margin: -50px auto 1rem auto;
}

@keyframes pulse {
    0% {
        box-shadow: 0 0 0 0 rgba(59, 130, 246, 0.4);
    }
    70% {
        box-shadow: 0 0 0 10px rgba(59, 130, 246, 0);
    }
    100% {
        box-shadow: 0 0 0 0 rgba(59, 130, 246, 0);
    }
}

@media (max-width: 768px) {
    .hero-section {
        padding: 2rem 1rem;
        margin: -1rem -1rem 2rem -1rem;
    }

    .hero-section h1 {
        font-size: 1.75rem;
    }

    .phase-wrapper {
        flex-direction: column;
    }

    .timeline-line {
        width: 4px;
        height: 100%;
        left: 23px;
        top: 0;
        transform: none;
    }

    .phase {
        display: flex;
        align-items: center;
        text-align: left;
        padding: 1rem 0 1rem 60px;
    }

    .phase-marker {
        position: absolute;
        left: 0;
        margin: 0;
    }

    .phase-content {
        margin-left: 1rem;
    }
}
</style>

<div class="hero-section">
    <h1>Welcome to Your SNWG Assessment Journey!</h1>
    <p>Your guide to navigating the assessment process successfully</p>
</div>

## Your Assessment Progress

Track your journey through each phase of the assessment process:

<div class="timeline">
    <div class="timeline-line"></div>
    <div class="phase-wrapper">
        <div class="phase completed">
            <div class="phase-marker">✓</div>
            <div class="phase-content">
                <h3>Getting Started</h3>
                <p>Complete onboarding</p>
            </div>
        </div>
        <div class="phase current">
            <div class="phase-marker">2</div>
            <div class="phase-content">
                <h3>Survey Review</h3>
                <p>Analyze agency needs</p>
            </div>
        </div>
        <div class="phase">
            <div class="phase-marker">3</div>
            <div class="phase-content">
                <h3>Agency Interviews</h3>
                <p>Gather insights</p>
            </div>
        </div>
        <div class="phase">
            <div class="phase-marker">4</div>
            <div class="phase-content">
                <h3>Solution Development</h3>
                <p>Propose recommendations</p>
            </div>
        </div>
    </div>
</div>

## You Are Here: Survey Review Phase

<div class="action-grid">
    <div class="action-card">
        <h3>📋 Take Action Now</h3>
        <ul>
            <li>Read assigned survey responses</li>
            <li>Review previous cycle information</li>
            <li>Identify key questions for agency</li>
            <li>Schedule pre-interview huddle</li>
            <li>Complete training modules</li>
        </ul>
    </div>
    
    <div class="action-card">
        <h3>📅 Coming Up Next</h3>
        <ul>
            <li>Agency interviews (2-3 weeks)</li>
            <li>Document initial findings</li>
            <li>Begin solution brainstorming</li>
            <li>Team collaboration sessions</li>
        </ul>
    </div>
</div>

## Key Resources

<div class="resource-grid">
    <div class="resource-card">
        <div class="resource-icon">📚</div>
        <h4>Survey Analysis Guide</h4>
        <p>Best practices for reviewing and analyzing agency survey responses</p>
        <a href="#" class="btn btn-primary btn-sm">View Guide</a>
    </div>
    
    <div class="resource-card">
        <div class="resource-icon">👥</div>
        <h4>Interview Preparation</h4>
        <p>Tips and templates for effective agency interviews</p>
        <a href="#" class="btn btn-primary btn-sm">View Guide</a>
    </div>
    
    <div class="resource-card">
        <div class="resource-icon">📊</div>
        <h4>Previous Cycle Examples</h4>
        <p>Learn from past successful assessments</p>
        <a href="#" class="btn btn-primary btn-sm">View Examples</a>
    </div>
</div>

## Timeline & Key Dates

<table class="timeline-table">
    <tr>
        <td>Survey Review Completion</td>
        <td>Jan 15, 2025</td>
        <td><span class="status-badge in-progress">In Progress</span></td>
    </tr>
    <tr>
        <td>Agency Interviews Begin</td>
        <td>Feb 1, 2025</td>
        <td><span class="status-badge upcoming">Upcoming</span></td>
    </tr>
    <tr>
        <td>Initial Findings Due</td>
        <td>Feb 28, 2025</td>
        <td><span class="status-badge upcoming">Upcoming</span></td>
    </tr>
    <tr>
        <td>Solution Development</td>
        <td>Mar 15, 2025</td>
        <td><span class="status-badge upcoming">Upcoming</span></td>
    </tr>
</table>

## Tips for Success

1. Start reviewing surveys early to identify patterns and key themes
2. Document questions and insights in Asana as you review
3. Connect with your thematic area lead for guidance
4. Attend all scheduled training sessions
5. Reach out to SNWG MO if you need support

<div class="help-container">
    <div class="help-icon">💡</div>
    <h3>Need Help?</h3>
    <p>The SNWG Management Office is here to support you throughout the assessment process.</p>
    <p>Contact us at: <a href="mailto:info@snwg-impact.net">info@snwg-impact.net</a></p>
</div>

<script>
document.addEventListener('DOMContentLoaded', () => {
    // Add hover effects and animation triggers
    const cards = document.querySelectorAll('.action-card, .resource-card');
    
    cards.forEach(card => {
        card.addEventListener('mouseenter', () => {
            card.style.transform = 'translateY(-5px)';
        });
        
        card.addEventListener('mouseleave', () => {
            card.style.transform = 'translateY(0)';
        });
    });
});
</script>