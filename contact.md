---
layout: default
title: Contact
permalink: /contact/
---

<section class="section">
    <div class="container">
        <h1 class="section-title">Get In Touch</h1>
        <p class="section-subtitle">
            Ready to transform your IT infrastructure? Let's start the conversation.
        </p>
        
        <div style="max-width: 800px; margin: 0 auto;">
            <div class="card-grid" style="grid-template-columns: 1fr 1fr; margin-bottom: 3rem;">
                <div class="card">
                    <div class="card-icon">
                        <i class="fas fa-envelope"></i>
                    </div>
                    <h3 class="card-title">Email Us</h3>
                    <p class="card-description">
                        <a href="mailto:{{ site.email }}">{{ site.email }}</a>
                    </p>
                </div>
                
                <div class="card">
                    <div class="card-icon">
                        <i class="fas fa-phone"></i>
                    </div>
                    <h3 class="card-title">Call Us</h3>
                    <p class="card-description">
                        <a href="tel:+44123351500">01233 51500</a>
                    </p>
                </div>
            </div>
            
            <div class="card">
                <h3 class="card-title" style="text-align: center; margin-bottom: 2rem;">Send us a Message</h3>
                <form id="contact-form" action="https://formspree.io/f/xnngdrlg" method="POST" style="max-width: 600px; margin: 0 auto;">
                    <!-- Hidden fields for Formspree -->
                    <input type="hidden" name="_subject" value="New Contact Form Submission from LJ Consulting Website" />
                    <input type="hidden" name="_next" value="https://ljconsulting.uk/contact/?success=true" />
                    <input type="hidden" name="_captcha" value="false" />
                    
                    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; margin-bottom: 1rem;">
                        <div>
                            <label for="firstName" style="display: block; margin-bottom: 0.5rem; color: var(--text-primary);">First Name *</label>
                            <input type="text" id="firstName" name="firstName" required 
                                   style="width: 100%; padding: 1rem; border: 1px solid var(--border-color); 
                                          border-radius: 10px; background: var(--card-bg); color: var(--text-primary); 
                                          font-size: 1rem; transition: var(--transition-fast);"
                                   onfocus="this.style.borderColor='var(--primary-color)'"
                                   onblur="this.style.borderColor='var(--border-color)'">
                        </div>
                        <div>
                            <label for="lastName" style="display: block; margin-bottom: 0.5rem; color: var(--text-primary);">Last Name *</label>
                            <input type="text" id="lastName" name="lastName" required 
                                   style="width: 100%; padding: 1rem; border: 1px solid var(--border-color); 
                                          border-radius: 10px; background: var(--card-bg); color: var(--text-primary); 
                                          font-size: 1rem; transition: var(--transition-fast);"
                                   onfocus="this.style.borderColor='var(--primary-color)'"
                                   onblur="this.style.borderColor='var(--border-color)'">
                        </div>
                    </div>
                    
                    <div style="margin-bottom: 1rem;">
                        <label for="email" style="display: block; margin-bottom: 0.5rem; color: var(--text-primary);">Email Address *</label>
                        <input type="email" id="email" name="email" required 
                               style="width: 100%; padding: 1rem; border: 1px solid var(--border-color); 
                                      border-radius: 10px; background: var(--card-bg); color: var(--text-primary); 
                                      font-size: 1rem; transition: var(--transition-fast);"
                               onfocus="this.style.borderColor='var(--primary-color)'"
                               onblur="this.style.borderColor='var(--border-color)'">
                    </div>
                    
                    <div style="margin-bottom: 1rem;">
                        <label for="company" style="display: block; margin-bottom: 0.5rem; color: var(--text-primary);">Company</label>
                        <input type="text" id="company" name="company" 
                               style="width: 100%; padding: 1rem; border: 1px solid var(--border-color); 
                                      border-radius: 10px; background: var(--card-bg); color: var(--text-primary); 
                                      font-size: 1rem; transition: var(--transition-fast);"
                               onfocus="this.style.borderColor='var(--primary-color)'"
                               onblur="this.style.borderColor='var(--border-color)'">
                    </div>
                    
                    <div style="margin-bottom: 1rem;">
                        <label for="service" style="display: block; margin-bottom: 0.5rem; color: var(--text-primary);">Service Interest</label>
                        <select id="service" name="service" 
                                style="width: 100%; padding: 1rem; border: 1px solid var(--border-color); 
                                       border-radius: 10px; background: var(--card-bg); color: var(--text-primary); 
                                       font-size: 1rem; transition: var(--transition-fast);"
                                onfocus="this.style.borderColor='var(--primary-color)'"
                                onblur="this.style.borderColor='var(--border-color)'">
                            <option value="">Select a service</option>
                            <option value="microsoft">Microsoft Products</option>
                            <option value="azure">Azure Cloud</option>
                            <option value="infrastructure">Infrastructure</option>
                            <option value="security">Security Solutions</option>
                            <option value="avd">Azure Virtual Desktop</option>
                            <option value="support">Support & Maintenance</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                    
                    <div style="margin-bottom: 2rem;">
                        <label for="message" style="display: block; margin-bottom: 0.5rem; color: var(--text-primary);">Message *</label>
                        <textarea id="message" name="message" rows="5" required 
                                  style="width: 100%; padding: 1rem; border: 1px solid var(--border-color); 
                                         border-radius: 10px; background: var(--card-bg); color: var(--text-primary); 
                                         font-size: 1rem; transition: var(--transition-fast); resize: vertical;"
                                  onfocus="this.style.borderColor='var(--primary-color)'"
                                  onblur="this.style.borderColor='var(--border-color)'"
                                  placeholder="Tell us about your project or requirements..."></textarea>
                    </div>
                    
                    <div style="text-align: center;">
                        <button type="submit" class="btn btn-primary" style="width: 100%; max-width: 300px;">
                            <i class="fas fa-paper-plane" style="margin-right: 0.5rem;"></i>
                            Send Message
                        </button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</section>

<section class="section" style="background: var(--card-bg);">
    <div class="container">
        <h2 class="section-title">Why Choose LJ Consulting?</h2>
        <div class="card-grid">
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-rocket"></i>
                </div>
                <h3 class="card-title">Fast Response</h3>
                <p class="card-description">
                    We respond to all inquiries within 24 hours and provide 
                    detailed project proposals within 48 hours.
                </p>
            </div>
            
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-handshake"></i>
                </div>
                <h3 class="card-title">Free Consultation</h3>
                <p class="card-description">
                    Initial consultation and project assessment are always 
                    free with no obligation to proceed.
                </p>
            </div>
            
            <div class="card">
                <div class="card-icon">
                    <i class="fas fa-shield-check"></i>
                </div>
                <h3 class="card-title">Guaranteed Results</h3>
                <p class="card-description">
                    We stand behind our work with comprehensive warranties 
                    and ongoing support for all implementations.
                </p>
            </div>
        </div>
    </div>
</section>
