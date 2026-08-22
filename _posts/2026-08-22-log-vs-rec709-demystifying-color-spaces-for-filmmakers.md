---
layout: post
title: "Log vs. Rec.709: Demystifying Color Spaces for Filmmakers"
description: "Understand log vs rec709 shooting for better color and dynamic range. Learn when to use each for your filmmaking projects."
date: 2026-08-22
categories: [post-production]
tags: [log vs rec709 shooting, color spaces, dynamic range, filmmaking tips, post-production]
---
You need to understand the difference between log and Rec.709 color spaces if you want to control your image. Too many new filmmakers just hit record without thinking about their camera's color settings. But choosing the right color space *before* you start shooting makes a huge difference in post-production. This isn't just theory; it directly impacts how much you can manipulate your footage later. Knowing when and why to use log vs rec709 shooting is a fundamental skill.

## What is Rec.709? Your Everyday Standard

Let's start with Rec.709 because it's probably what you're most familiar with, even if you don't know the name. Rec.709 is the standard color space for television, Blu-ray, and most web content. It's designed to look good right out of the camera, on consumer monitors, without any heavy grading.

Think of it like this: your iPhone shoots in something very close to Rec.709. When you watch Netflix, YouTube, or broadcast TV, you're looking at Rec.709 footage. It has a specific contrast ratio and color saturation that's optimized for displays that aren't necessarily calibrated for high dynamic range.

**Pros of Shooting in Rec.709:**

*   **Ready-to-use footage:** Your clips look good instantly. This is perfect for quick turnaround projects, vlogs, or documentary work where you don't have a lot of post-production time.
*   **Easier for beginners:** Less to worry about in post. What you see is pretty much what you get.
*   **Smaller file sizes (sometimes):** Because it captures less dynamic range and color information, the files can be smaller than log files, though this varies by camera and codec.

**Cons of Shooting in Rec.709:**

*   **Limited dynamic range:** This is the big one. Rec.709 compresses the highlights and shadows into a narrower range. If you shoot a bright sky and a dark foreground, you're likely to blow out the sky or crush the shadows. There's not much detail to recover.
*   **Less color grading flexibility:** You have less room to push and pull colors in post. If your white balance is off, it's harder to fix without introducing color shifts or artifacts.

**When to Use Rec.709:**

Shoot Rec.709 when you need to turn around footage fast, have controlled lighting, or are delivering directly to a standard Rec.709 display without much grading. Think corporate interviews in a studio, news packages, or simple home videos. If you're shooting an event with varied light and can't control it, but your delivery is fast, Rec.709 might be a pragmatic choice to avoid post-production headaches, even if it sacrifices image quality.

## What is Log? Capturing More Information

Log, short for "logarithmic," is a flat, desaturated image profile designed to capture the maximum amount of dynamic range and color information from your camera's sensor. Instead of squeezing the image into a display-ready format, log spreads the light information out across the available digital range. This preserves detail in both the brightest highlights and the darkest shadows.

Every major camera manufacturer has their own version of log: Sony has S-Log (S-Log2, S-Log3), Canon has C-Log, Panasonic has V-Log, ARRI has Log-C, RED has Log3G10, etc. While they all have slightly different characteristics, their purpose is the same: maximize the data.

When you look at log footage straight out of the camera, it looks flat, grey, and desaturated. It often looks underexposed. This is intentional. It's not meant to be viewed directly; it's meant to be graded.

**Pros of Shooting in Log:**

*   **Massive dynamic range:** This is the main reason to shoot log. You can capture much more detail in bright skies and deep shadows, giving you more flexibility in post to pull that detail back. Think of it like a digital negative.
*   **Greater color grading flexibility:** Because log captures more color information, you have more room to adjust saturation, hue, and luminance without breaking the image. You can craft specific looks, match different cameras, and correct color issues more robustly.
*   **Matches higher-end workflows:** If you're aiming for a cinematic look, log is the standard. It gives you the raw material to achieve that polished, filmic finish.

**Cons of Shooting in Log:**

*   **Requires post-production:** Log footage *must* be color graded. You can't just deliver it straight from the camera. This adds time and skill requirements to your workflow.
*   **Can be difficult to monitor:** Viewing flat log footage on set can make it hard to judge exposure and color accurately. You often need external monitors with LUT (Look Up Table) support to preview a graded image.
*   **Noise in shadows if underexposed:** Log profiles are often designed with a slight bias towards preserving highlights. If you underexpose log footage, especially S-Log3 or V-Log, you can introduce noticeable noise in the shadows when you try to lift them in post. This is a common mistake for new filmmakers.

**When to Use Log:**

Shoot log when you want maximum control over your image in post, when you're shooting in high-contrast environments (bright sun, deep shadows), or when you're aiming for a cinematic look. It's essential for narrative films, commercials, music videos, or any project where precise color grading is critical.

## The Exposure Difference: A Critical Point for Log

This is where many new filmmakers get tripped up. The optimal exposure for log vs rec709 shooting is different.

**Rec.709 Exposure:** You expose Rec.709 pretty much how you want the final image to look. If a shot looks good on your monitor, it's likely properly exposed.

**Log Exposure (Overexpose by a stop or two):** This is a widely adopted practice for most log profiles from Sony, Panasonic, and Canon. You often want to expose log footage brighter than it looks good on your monitor. Why? Because log profiles are usually designed to protect highlights more than shadows. By exposing a stop or two brighter (often called "exposing to the right" or ETTR), you push the shadow information further away from the noise floor of the sensor. This gives you cleaner shadows when you bring the exposure down in post.

For example, if you're shooting on a Sony FX3 with S-Log3, you might aim for skin tones to be around 60-70% on a waveform monitor, rather than the 50% you might target for Rec.709. This slightly overexposed look will appear "correct" once you apply a LUT and color grade.

**Practical Tip:** When shooting log, always use a waveform monitor, zebras, or false color. Don't rely solely on your eye on a flat log image. Learn what optimal exposure looks like on your camera's log profile using these tools. If you're looking for real-time feedback on your exposure settings while you shoot, [FrameCoach](https://framecoach.io) gives you that coaching layer right on your phone, helping you nail those log exposures without guesswork.

## How LUTs Fit In

LUTs (Look Up Tables) are a critical part of the log workflow. They serve two main purposes:

1.  **Monitoring LUTs:** These are applied in-camera or on an external monitor to convert the flat log image into something that looks closer to a finished Rec.709 image. This helps you and your crew judge exposure, focus, and composition more accurately on set. It's a preview, not baked into the footage.
2.  **Conversion LUTs (or Base LUTs):** These are applied in your editing software (DaVinci Resolve, Premiere Pro, etc.) to transform your log footage into a standard Rec.709 color space. This is usually the first step in your color grading process. After applying this base LUT, you then perform your creative grade on top of it. Many camera manufacturers provide official conversion LUTs for their log profiles.

You don't just throw any LUT on any log footage. Make sure you're using the correct conversion LUT for your specific camera's log profile (e.g., S-Log3 to Rec.709, C-Log2 to Rec.709). Using the wrong LUT will give you incorrect colors and contrast.

## The Hybrid Approach: Why Some Cameras Offer Both

Some cameras offer profiles that are somewhere in between full log and Rec.709. Panasonic's V-Log L (for GH series) or Sony's HLG (Hybrid Log Gamma) are examples. HLG is designed to be displayed directly on HDR televisions, offering more dynamic range than Rec.709 without requiring extensive grading. It's a 'delivery-ready' HDR format. For serious cinematic work, you'll still lean towards full log, but these hybrid options are becoming more common for workflows that prioritize speed and modern display compatibility.

## Making the Call: Log vs. Rec.709 Shooting

The choice comes down to your project's needs, your time in post, and your desired final look.

**Choose Rec.709 if:**

*   Your delivery timeline is tight.
*   You have limited post-production resources or skill.
*   Lighting conditions are controlled and consistent.
*   Your project doesn't demand extensive color grading (e.g., news, event coverage).
*   You are shooting for immediate public consumption without much fuss, like a social media update.

**Choose Log if:**

*   You want maximum image quality and dynamic range.
*   You plan to do extensive color grading to create a specific look.
*   You're shooting in high-contrast environments.
*   You need to match footage from different cameras.
*   Your project requires a cinematic, polished aesthetic.

For instance, shooting a narrative short film with a high dynamic range scene—say, an interior with bright windows—demands log. You'd shoot S-Log3 on an FX6, expose carefully with a waveform, and then bring it into Resolve to apply a base LUT and craft your look. For a quick interview shot against a controlled backdrop with a single LED, Rec.709 would be completely fine and save you time.

Understanding the principles of log vs rec709 shooting is key to unlocking the full potential of your camera and your post-production workflow. It's not about one being inherently "better" than the other, but about using the right tool for the right job. If you're serious about your craft, taking the time to master log exposure and grading will elevate your work significantly. For practical exercises and monitoring assistance, remember that [FrameCoach](https://framecoach.io) can be a powerful tool for learning how to expose correctly in various shooting conditions.

Start by shooting a test with both profiles. Take your camera, find a high-contrast scene, and shoot a few clips in Rec.709 and then the equivalent in your camera's log profile. Bring both into your editing software, apply a basic conversion LUT to the log footage, and see how much more flexibility you have with the log files. Pay attention to the highlight and shadow detail. This hands-on comparison will solidify your understanding more than any blog post can.