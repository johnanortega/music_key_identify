# Info:

This is a test of the audio processing for the songs "Gotta Feeling by Black Eyed Peas", "Prendio by Omar Montes" and "Princesas by Pereza". The table below shows the results of the key estimation using different parameters for the Fourier Transform (n_fft and hop_length), CQT and CENS chromagrams with hop_length. The key is estimated using the Short-Time Fourier Transform (STFT), Constant Q Transform (CQT), and Chroma Energy Normalized Statistics (CENS). The elapsed time for each method is also recorded. Key estimates from other sources are also included for comparison (VDJ, Serato, Rekordbox, TunesBat-SpotifyAPI, Essentia...).

Tests have been carried out using correlation algorithms such as Krumhansl and Temperley for the song "Princesas by Pereza" for Short-Time Fourier Transform (STFT), Constant Q Transform (CQT), and Chroma Energy Normalized Statistics (CENS). It can be seen that the data completely differs from those obtained by the chromagrams. See table in "Pereza - Princesas".

# Conclusion:

The best identification of musical keys is evidenced using the methodology of chromagram-based methods, as can be seen in the published audio.

Using Pearson-based correlations, data close to the expected data that chromagram-based methods return are obtained.

The analysis times are much lower for chromagram-based methods than for the use of correlations, with the values being more faithful for chromagrams only.

# Results:

## Mashup result: [Link to YouTube](https://www.youtube.com/watch?v=WjzdnwJ_XBk)

## Black Eyed Peas - Gotta Feeling

- VDJ:        Instrumental 6A / Original 6A
- Serato:     Instrumental 9A / Original 9A
- Rekordbox:  Instrumental 9A / Original 9A
- TunesBat:   Original 6A
- Essentia:   Instrumental 8B / Original 8B

    *Instrumental*

    | n_fft | hop_length | estimate_key_stft                      | estimate_key_cqt                       | estimate_key_cens                      | elapsed_time_stft | elapsed_time_cqt | elapsed_time_cens |
    |-------|------------|----------------------------------------|----------------------------------------|----------------------------------------|-------------------|------------------|-------------------|
    | 1024  | 1024       | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 5.568944          | -                | -                 |
    | 1024  | 2048       | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 4.37303           | -                | -                 |
    | 1024  | 4096       | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 4.432682          | -                | -                 |
    | 1024  | 8192       | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 4.249945          | -                | -                 |
    | 1024  | 16384      | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 4.251495          | -                | -                 |
    | 2048  | 1024       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.908215          | -                | -                 |
    | 2048  | 2048       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.467983          | -                | -                 |
    | 2048  | 4096       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.493951          | -                | -                 |
    | 2048  | 8192       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.40272           | -                | -                 |
    | 2048  | 16384      | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.548333          | -                | -                 |
    | 4096  | 1024       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 5.596528          | -                | -                 |
    | 4096  | 2048       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.917618          | -                | -                 |
    | 4096  | 4096       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.578552          | -                | -                 |
    | 4096  | 8192       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.495243          | -                | -                 |
    | 4096  | 16384      | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.509029          | -                | -                 |
    | 8192  | 1024       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 7.462399          | -                | -                 |
    | 8192  | 2048       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 5.790958          | -                | -                 |
    | 8192  | 4096       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.990726          | -                | -                 |
    | 8192  | 8192       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.714767          | -                | -                 |
    | 8192  | 16384      | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.411374          | -                | -                 |
    | 16384 | 1024       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 10.813032         | -                | -                 |
    | 16384 | 2048       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 7.181766          | -                | -                 |
    | 16384 | 4096       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 5.699495          | -                | -                 |
    | 16384 | 8192       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.858667          | -                | -                 |
    | 16384 | 16384      | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.539086          | -                | -                 |
    | -     | 1024       | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 3.184163         | 2.778847          |
    | -     | 2048       | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 2.37866          | 2.597833          |
    | -     | 4096       | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 2.339809         | 2.608254          |
    | -     | 8192       | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 2.090203         | 2.471206          |
    | -     | 16384      | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 2.180459         | 2.69416           |

## Omar Montes - Prendio

- VDJ:        Instrumental 9A / Vocal 10A / Original 9A
- Serato:     Instrumental 9A / Vocal 9A  / Original 9A
- Rekordbox:  Instrumental 9A / Vocal 9B  / Original 9A
- TunesBat:   Original 9A
- Essentia:   Instrumental 9A / Original 9A

    *Instrumental*

    | n_fft | hop_length | estimate_key_stft                      | estimate_key_cqt                       | estimate_key_cens                      | elapsed_time_stft | elapsed_time_cqt | elapsed_time_cens |
    |-------|------------|----------------------------------------|--------------------------------------- |----------------------------------------|------------------ |----------------- |-------------------|
    | 1024  | 1024       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 4.231483          | -                | -                 |
    | 1024  | 2048       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 2.827105          | -                | -                 |
    | 1024  | 4096       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 2.915388          | -                | -                 |
    | 1024  | 8192       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 2.915934          | -                | -                 |
    | 1024  | 16384      | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 2.639825          | -                | -                 |
    | 2048  | 1024       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.17459           | -                | -                 |
    | 2048  | 2048       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.125024          | -                | -                 |
    | 2048  | 4096       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.106008          | -                | -                 |
    | 2048  | 8192       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.508087          | -                | -                 |
    | 2048  | 16384      | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.13598           | -                | -                 |
    | 4096  | 1024       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.895818          | -                | -                 |
    | 4096  | 2048       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 5.412757          | -                | -                 |
    | 4096  | 4096       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 4.096375          | -                | -                 |
    | 4096  | 8192       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 4.050407          | -                | -                 |
    | 4096  | 16384      | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 2.939166          | -                | -                 |
    | 8192  | 1024       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 6.442189          | -                | -                 |
    | 8192  | 2048       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 4.161694          | -                | -                 |
    | 8192  | 4096       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.633629          | -                | -                 |
    | 8192  | 8192       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.127671          | -                | -                 |
    | 8192  | 16384      | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 2.931342          | -                | -                 |
    | 16384 | 1024       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 7.496297          | -                | -                 |
    | 16384 | 2048       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 5.130757          | -                | -                 |
    | 16384 | 4096       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 4.042871          | -                | -                 |
    | 16384 | 8192       | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.741376          | -                | -                 |
    | 16384 | 16384      | Nomenclature: E Minor, Camelot Key: 9A | -                                      | -                                      | 3.207464          | -                | -                 |
    | -     | 1024       | -                                      | Nomenclature: E Minor, Camelot Key: 9A | Nomenclature: E Minor, Camelot Key: 9A | -                 | 1.867911         | 1.688501          |
    | -     | 2048       | -                                      | Nomenclature: E Minor, Camelot Key: 9A | Nomenclature: E Minor, Camelot Key: 9A | -                 | 1.720101         | 1.701225          |
    | -     | 4096       | -                                      | Nomenclature: E Minor, Camelot Key: 9A | Nomenclature: E Minor, Camelot Key: 9A | -                 | 1.266177         | 1.608956          |
    | -     | 8192       | -                                      | Nomenclature: E Minor, Camelot Key: 9A | Nomenclature: E Minor, Camelot Key: 9A | -                 | 1.292229         | 1.77314           |
    | -     | 16384      | -                                      | Nomenclature: E Minor, Camelot Key: 9A | Nomenclature: E Minor, Camelot Key: 9A | -                 | 1.334187         | 1.812899          |

    *Vocal*

    | n_fft | hop_length | estimate_key_stft                      | estimate_key_cqt                       | estimate_key_cens                      | elapsed_time_stft | elapsed_time_cqt | elapsed_time_cens |
    |-------|------------|----------------------------------------|--------------------------------------- |----------------------------------------|------------------ |----------------- |-------------------|
    | 1024  | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.231483          | -                | -                 |
    | 1024  | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.827105          | -                | -                 |
    | 1024  | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.915388          | -                | -                 |
    | 1024  | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.915934          | -                | -                 |
    | 1024  | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.639825          | -                | -                 |
    | 2048  | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.17459           | -                | -                 |
    | 2048  | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.125024          | -                | -                 |
    | 2048  | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.106008          | -                | -                 |
    | 2048  | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.508087          | -                | -                 |
    | 2048  | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.13598           | -                | -                 |
    | 4096  | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.895818          | -                | -                 |
    | 4096  | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 5.412757          | -                | -                 |
    | 4096  | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.096375          | -                | -                 |
    | 4096  | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.050407          | -                | -                 |
    | 4096  | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.939166          | -                | -                 |
    | 8192  | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 6.442189          | -                | -                 |
    | 8192  | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.161694          | -                | -                 |
    | 8192  | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.633629          | -                | -                 |
    | 8192  | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.127671          | -                | -                 |
    | 8192  | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.931342          | -                | -                 |
    | 16384 | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 7.496297          | -                | -                 |
    | 16384 | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 5.130757          | -                | -                 |
    | 16384 | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.042871          | -                | -                 |
    | 16384 | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.741376          | -                | -                 |
    | 16384 | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.207464          | -                | -                 |
    | -     | 1024       | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.867911         | 1.688501          |
    | -     | 2048       | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.720101         | 1.701225          |
    | -     | 4096       | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.266177         | 1.608956          |
    | -     | 8192       | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.292229         | 1.77314           |
    | -     | 16384      | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.334187         | 1.812899          |

    *Vocal without multisegments (best times)*

    | n_fft   |   hop_length | estimate_key_stft                      | estimate_key_cqt                       | estimate_key_cens                      | elapsed_time_stft   | elapsed_time_cqt   | elapsed_time_cens   |
    |:--------|-------------:|:---------------------------------------|:---------------------------------------|:---------------------------------------|:--------------------|:-------------------|:--------------------|
    | 1024    |         1024 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 1.5295500755310059  | -                  | -                   |
    | 1024    |         2048 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.3895730972290039  | -                  | -                   |
    | 1024    |         4096 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.30129051208496094 | -                  | -                   |
    | 1024    |         8192 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.2357769012451172  | -                  | -                   |
    | 1024    |        16384 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.22298598289489746 | -                  | -                   |
    | 2048    |         1024 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.6069159507751465  | -                  | -                   |
    | 2048    |         2048 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.3801586627960205  | -                  | -                   |
    | 2048    |         4096 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.3127894401550293  | -                  | -                   |
    | 2048    |         8192 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.32311081886291504 | -                  | -                   |
    | 2048    |        16384 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.2948777675628662  | -                  | -                   |
    | 4096    |         1024 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 1.040912389755249   | -                  | -                   |
    | 4096    |         2048 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.6197991371154785  | -                  | -                   |
    | 4096    |         4096 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.45433497428894043 | -                  | -                   |
    | 4096    |         8192 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.37546539306640625 | -                  | -                   |
    | 4096    |        16384 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.2562274932861328  | -                  | -                   |
    | 8192    |         1024 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 2.5940887928009033  | -                  | -                   |
    | 8192    |         2048 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 1.3133511543273926  | -                  | -                   |
    | 8192    |         4096 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.9508144855499268  | -                  | -                   |
    | 8192    |         8192 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.4454634189605713  | -                  | -                   |
    | 8192    |        16384 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.32474589347839355 | -                  | -                   |
    | 16384   |         1024 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 5.076807737350464   | -                  | -                   |
    | 16384   |         2048 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 2.4823694229125977  | -                  | -                   |
    | 16384   |         4096 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 1.4458842277526855  | -                  | -                   |
    | 16384   |         8192 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.665252685546875   | -                  | -                   |
    | 16384   |        16384 | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 0.48616456985473633 | -                  | -                   |
    | -       |         1024 | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                   | 1.983579158782959  | 1.7017123699188232  |
    | -       |         2048 | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                   | 1.4300668239593506 | 1.4974634647369385  |
    | -       |         4096 | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                   | 1.5919239521026611 | 1.3956568241119385  |
    | -       |         8192 | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                   | 1.3495135307312012 | 1.5055642127990723  |
    | -       |        16384 | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                   | 1.3229587078094482 | 1.7234458923339844  |    
    

## Pereza - Princesas

- VDJ:        Instrumental 9B / Vocal 10B / Original 9B
- Serato:     Instrumental 9B / Vocal 9A  / Original 9B
- Rekordbox:  Instrumental 9B / Vocal 9B  / Original 9B
- TunesBat:   Original 9B
- Essentia:   Instrumental 9B / Vocal 9B / Original 9B

    *Instrumental*

    | n_fft | hop_length | estimate_key_stft                      | estimate_key_cqt                       | estimate_key_cens                      | elapsed_time_stft | elapsed_time_cqt | elapsed_time_cens |
    |-------|------------|----------------------------------------|--------------------------------------- |----------------------------------------|------------------ |----------------- |-------------------|
    | 1024  | 1024       | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 4.231483          | -                | -                 |
    | 1024  | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.827105          | -                | -                 |
    | 1024  | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.915388          | -                | -                 |
    | 1024  | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.915934          | -                | -                 |
    | 1024  | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.639825          | -                | -                 |
    | 2048  | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.17459           | -                | -                 |
    | 2048  | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.125024          | -                | -                 |
    | 2048  | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.106008          | -                | -                 |
    | 2048  | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.508087          | -                | -                 |
    | 2048  | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.13598           | -                | -                 |
    | 4096  | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.895818          | -                | -                 |
    | 4096  | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 5.412757          | -                | -                 |
    | 4096  | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.096375          | -                | -                 |
    | 4096  | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.050407          | -                | -                 |
    | 4096  | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.939166          | -                | -                 |
    | 8192  | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 6.442189          | -                | -                 |
    | 8192  | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.161694          | -                | -                 |
    | 8192  | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.633629          | -                | -                 |
    | 8192  | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.127671          | -                | -                 |
    | 8192  | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 2.931342          | -                | -                 |
    | 16384 | 1024       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 7.496297          | -                | -                 |
    | 16384 | 2048       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 5.130757          | -                | -                 |
    | 16384 | 4096       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 4.042871          | -                | -                 |
    | 16384 | 8192       | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.741376          | -                | -                 |
    | 16384 | 16384      | Nomenclature: E Minor, Camelot Key: 9B | -                                      | -                                      | 3.207464          | -                | -                 |
    | -     | 1024       | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.867911         | 1.688501          |
    | -     | 2048       | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.720101         | 1.701225          |
    | -     | 4096       | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.266177         | 1.608956          |
    | -     | 8192       | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.292229         | 1.77314           |
    | -     | 16384      | -                                      | Nomenclature: E Minor, Camelot Key: 9B | Nomenclature: E Minor, Camelot Key: 9B | -                 | 1.334187         | 1.812899          |

    *Vocal*

    | n_fft | hop_length | estimate_key_stft                      | estimate_key_cqt                       | estimate_key_cens                      | elapsed_time_stft | elapsed_time_cqt | elapsed_time_cens |
    |-------|------------|----------------------------------------|--------------------------------------- |----------------------------------------|------------------ |----------------- |-------------------|    
    | 1024  | 1024       | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 4.54651           | -                | -                 |
    | 1024  | 2048       | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 3.25916           | -                | -                 |
    | 1024  | 4096       | Nomenclature: G Minor, Camelot Key: 6A | -                                      | -                                      | 3.148158          | -                | -                 |
    | 1024  | 8192       | Nomenclature: A Minor, Camelot Key: 8A | -                                      | -                                      | 3.300642          | -                | -                 |
    | 1024  | 16384      | Nomenclature: G# Minor, Camelot Key: 1A| -                                      | -                                      | 3.130941          | -                | -                 |
    | 2048  | 1024       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.544903          | -                | -                 |
    | 2048  | 2048       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.589798          | -                | -                 |
    | 2048  | 4096       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.230793          | -                | -                 |
    | 2048  | 8192       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.186098          | -                | -                 |
    | 2048  | 16384      | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.176542          | -                | -                 |
    | 4096  | 1024       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.019447          | -                | -                 |
    | 4096  | 2048       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.637857          | -                | -                 |
    | 4096  | 4096       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.249382          | -                | -                 |
    | 4096  | 8192       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.244065          | -                | -                 |
    | 4096  | 16384      | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.2495            | -                | -                 |
    | 8192  | 1024       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 5.509722          | -                | -                 |
    | 8192  | 2048       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.371078          | -                | -                 |
    | 8192  | 4096       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.584513          | -                | -                 |
    | 8192  | 8192       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.424356          | -                | -                 |
    | 8192  | 16384      | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.11183           | -                | -                 |
    | 16384 | 1024       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 8.160713          | -                | -                 |
    | 16384 | 2048       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 5.568185          | -                | -                 |
    | 16384 | 4096       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 4.198343          | -                | -                 |
    | 16384 | 8192       | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.863103          | -                | -                 |
    | 16384 | 16384      | Nomenclature: G Major, Camelot Key: 9B | -                                      | -                                      | 3.455538          | -                | -                 |
    | -     | 1024       | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 2.291726         | 2.034826          |
    | -     | 2048       | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 2.072977         | 1.883194          |
    | -     | 4096       | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 1.549565         | 1.828388          |
    | -     | 8192       | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 1.600577         | 1.766589          |
    | -     | 16384      | -                                      | Nomenclature: G Major, Camelot Key: 9B | Nomenclature: G Major, Camelot Key: 9B | -                 | 1.610879         | 2.192974          |
    
    **Vocal based on correlation algorithms*

    _Best coincidence Krumhansl with pearson_

    | n_fft |   hop_length | test_chroma_krumhansl                      | test_chroma_temperley                        | test_chroma_krumhansl_pearson              | test_chroma_temperley_pearson                |   elapsed_time_krumhansl |   elapsed_time_temperley |   elapsed_time_krumhansl_pearson |   elapsed_time_temperley_pearson |
    |-------|--------------|--------------------------------------------|----------------------------------------------|--------------------------------------------|----------------------------------------------|--------------------------|--------------------------|----------------------------------|----------------------------------|
    |  1024 |         1024 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT F# Minor / CENS F# Minor  |                  6.43747 |                  4.60384 |                          4.90019 |                          4.74998 |
    |  1024 |         2048 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT F# Minor / CENS F# Minor  |                  3.75553 |                  4.35798 |                          4.443   |                          3.98346 |
    |  1024 |         4096 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT F# Minor / CENS F# Minor  |                  3.33343 |                  3.31504 |                          3.41994 |                          3.46527 |
    |  1024 |         8192 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT G Major / CENS G Major    |                  3.24044 |                  2.92703 |                          3.43279 |                          3.12495 |
    |  1024 |        16384 | STFT F# Minor / CQT G Minor / CENS B Minor | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT F# Minor / CQT G Major / CENS G Major | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  2.84283 |                  2.85626 |                          3.48786 |                          3.18371 |
    |  2048 |         1024 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT F# Minor / CENS F# Minor  |                  4.99233 |                  5.31658 |                          5.1198  |                          5.34533 |
    |  2048 |         2048 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT F# Minor / CENS F# Minor  |                  3.92779 |                  4.27245 |                          3.87338 |                          4.16175 |
    |  2048 |         4096 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT F# Minor / CENS F# Minor  |                  3.28846 |                  3.30289 |                          3.591   |                          3.5679  |
    |  2048 |         8192 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT G Major / CENS G Major    |                  3.50968 |                  3.48739 |                          3.36748 |                          3.10467 |
    |  2048 |        16384 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT G Minor / CQT F# Minor / CENS F# Minor  | STFT G Minor / CQT G Major / CENS G Major  | STFT G Minor / CQT F# Minor / CENS F# Minor  |                  2.8805  |                  2.753   |                          3.29553 |                          2.92743 |
    |  4096 |         1024 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  5.68463 |                  6.03148 |                          5.72975 |                          5.6398  |
    |  4096 |         2048 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  4.1953  |                  4.08372 |                          4.09733 |                          4.23593 |
    |  4096 |         4096 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  3.76004 |                  3.44689 |                          3.33639 |                          3.60136 |
    |  4096 |         8192 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT G Major / CENS G Major   |                  2.85943 |                  2.99059 |                          3.02284 |                          3.19453 |
    |  4096 |        16384 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  2.8712  |                  2.84661 |                          2.93645 |                          2.86485 |
    |  8192 |         1024 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  6.94546 |                  6.90049 |                          6.92023 |                          7.04514 |
    |  8192 |         2048 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  4.82391 |                  4.8938  |                          5.03711 |                          4.95787 |
    |  8192 |         4096 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  3.60968 |                  3.92869 |                          3.72772 |                          3.81953 |
    |  8192 |         8192 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT G Major / CENS G Major   |                  3.14092 |                  3.25258 |                          3.12696 |                          3.15217 |
    |  8192 |        16384 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  2.9848  |                  2.98735 |                          3.08389 |                          2.98882 |
    | 16384 |         1024 | STFT B Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT G Major / CQT F# Minor / CENS F# Minor  |                  9.69838 |                 10.4814  |                         12.0071  |                         14.1348  |
    | 16384 |         2048 | STFT B Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT G Major / CQT F# Minor / CENS F# Minor  |                  9.00082 |                  7.67391 |                          7.8031  |                          7.60822 |
    | 16384 |         4096 | STFT B Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT G Major / CQT F# Minor / CENS F# Minor  |                  5.6552  |                  5.60401 |                          5.59447 |                          5.28731 |
    | 16384 |         8192 | STFT B Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT G Major / CQT G Major / CENS G Major    |                  4.00256 |                  3.92397 |                          3.88214 |                          4.19688 |
    | 16384 |        16384 | STFT G Minor / CQT G Minor / CENS B Minor  | STFT F# Minor / CQT F# Minor / CENS F# Minor | STFT G Major / CQT G Major / CENS G Major  | STFT F# Minor / CQT F# Minor / CENS F# Minor |                  3.79524 |                  5.48979 |                          4.34324 |                          3.98776 |